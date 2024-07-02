# Running CUDA-Q on [Colab](https://colab.research.google.com/)

**Learn more about [CUDA-Q](https://developer.nvidia.com/cuda-q) with NVIDIA official [GitHub](https://github.com/NVIDIA/cuda-quantum/). Running the tutorials in the CUDA-Q container with the corresponding version `X.X.X` is highly recommended. Please follow the [instruction guide](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/quantum/containers/cuda-quantum) (Docker required).**
<br>
<br>
<br>
*Follow the steps below to run cudaq tutorials with free T4 GPU backend
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA-Q/assets/66664309/972d85f0-32f6-4ccc-9fc4-00b22804b434" width="800">
<br>
<br>
<br>

**Step 1. Log in [Colab](https://colab.research.google.com/) and click on the `open notebook` under the `file` tab**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/d96a3ae5-6110-4978-8d27-ff777d9c4014" width="800">
<br>
<br>
<br>

**Step 2. To access tutorials in this repository, search this repository in the `GitHub` catalog by typing:**
<br>
```
Squirtle007/CUDA-Q
```

**Then scroll down and click on the Colab tutorials with the desired version (ex. `0.7.1`)**
<img src="https://github.com/Squirtle007/CUDA-Q/assets/66664309/dfc5d2ca-9c3f-476d-a70c-090504deb8ac" width="800">
<br>
<br>
<br>

**Step 3. Make sure to select `Runtime > Change runtime type > T4 GPU` as the backend for acceleration**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/18685649-25e9-4a7e-b117-340063b3650f" width="800">
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/40e9d189-3a8d-4061-9f6e-5f9c98f12682" width="500">
<br>
<br>
<br>

**Step 4. Set up CUDA Quantum properly in the Colab environment using the following commands (at the very beginning)**
<br>
```
!wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/cuda-keyring_1.0-1_all.deb
!dpkg -i cuda-keyring_1.0-1_all.deb
!apt-get update
!apt-get -y install libcublas-11-8 libcusolver-11-8 cuda-cudart-11-8

%pip install cuda-quantum==0.6.0
```
<br>
<br>
<br>
