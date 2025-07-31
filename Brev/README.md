# 🚀 Launching CUDA-Q JupyterLab on Brev

This guide walks you through setting up a containerized CUDA-Q JupyterLab environment using [Brev](https://brev.nvidia.com/).

## Step 1: Login to Brev

Go to [https://brev.nvidia.com](https://brev.nvidia.com) and log in with your credentials.

---

## Step 2: Create a Launchable in Container Mode

* Click **“Create Launchable”**
* Choose **“Container”** mode
  ![Step 1](image.png)

---

## Step 3: Select Docker Compose

* Choose the **Docker Compose** option
* Click **“Add a container”**
  ![Step 2](image.png)

---

## Step 4: Specify the Container

* **Paste the CUDA-Q Docker image URL**

  ```bash
  nvcr.io/nvidia/quantum/cuda-quantum:cu12-0.11.0
  ```

* **Set the port mapping**

  ```bash
  8888:8888
  ```

  ![Step 3](image.png)

---

## Step 5: Add Custom Startup Command (IMPORTANT⚠️)

> Without this step, JupyterLab may open in an unexpected directory.

* Add the following command under the `Command` field:

  ```bash
  -c "jupyter lab --ip=0.0.0.0 --no-browser --NotebookApp.token='' --allow-root --NotebookApp.allow_origin='*' --notebook-dir='/home/cudaq'"
  ```

  ![Step 4](image.png)

---

## Step 6: Skip Jupyter Installation (IMPORTANT⚠️)

* When prompted: **Do not install Jupyter** again.
* Confirm the port `8888` is correctly mapped.
  ![Step 5](image.png)

---

## Step 7: Final Setup

* **Select a GPU** (many choices available)
* **Add storage**

  > **Recommended**: At least **50GB** to prevent Docker Compose failures
* **Name your Launchable**
* **Finish setup** — Your JupyterLab with CUDA-Q is ready to launch!

---

## ✅ Result

Once the container is launched, access **JupyterLab** via the provided Brev link at:

```
http://<your-brev-url>:8888
```

You're all set to start your CUDA-Q journey with **CUDA-Q** on Brev!

---

An example [Launchable](https://brev.nvidia.com/launchable/deploy/now?launchableID=env-2zjZhHYSKhrkSP2cidigUMIss9N).
