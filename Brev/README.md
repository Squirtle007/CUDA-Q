# 🚀 Launching CUDA-Q JupyterLab on Brev

This guide walks you through setting up a containerized CUDA-Q JupyterLab environment using [Brev](https://brev.nvidia.com/).

## Step 1: Login to Brev

Go to [https://brev.nvidia.com](https://brev.nvidia.com) and log in with your credentials, and click on `Create Launchable`.
<img width="1506" height="642" alt="image" src="https://github.com/user-attachments/assets/c60cbdce-f1c2-4cc7-8522-cc3daf50db48" />


---

## Step 2: Create a Launchable in Container Mode

* Click **“Create Launchable”**
* Choose **“Container”** mode
<img width="2239" height="971" alt="image" src="https://github.com/user-attachments/assets/7c872686-d7ca-47db-9e0d-2622971d0473" />


---

## Step 3: Select Docker Compose

* Choose the **Docker Compose** option
* Click **“Add a container”**
<img width="2452" height="1268" alt="image" src="https://github.com/user-attachments/assets/086b7a32-16c1-413c-a140-6c3337e5058e" />


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

<img width="2410" height="1229" alt="image" src="https://github.com/user-attachments/assets/00345f35-4fec-4da7-b08a-65ad32914139" />


---

## Step 5: Add Custom Startup Command (IMPORTANT⚠️)

> Without this step, JupyterLab may open in an unexpected directory.

* Add the following command under the `Command` field:

  ```bash
  -c "jupyter lab --ip=0.0.0.0 --no-browser --NotebookApp.token='' --allow-root --NotebookApp.allow_origin='*' --notebook-dir='/home/cudaq'"
  ```

<img width="2421" height="794" alt="image" src="https://github.com/user-attachments/assets/cf3c75be-96c2-4d31-b7a1-15cf94d365fb" />


---

## Step 6: Skip Jupyter Installation (IMPORTANT⚠️)

* When prompted: **Do not install Jupyter** again.
* Confirm the port `8888` is correctly mapped.
<img width="2429" height="1043" alt="image" src="https://github.com/user-attachments/assets/fa9293f4-8e09-4beb-b868-29383c374edb" />


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

➡️ Here is a pre-built [Launchable](https://brev.nvidia.com/launchable/deploy/now?launchableID=env-2zjZhHYSKhrkSP2cidigUMIss9N).
