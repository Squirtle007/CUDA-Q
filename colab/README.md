# Running CUDA-Q on [Colab](https://colab.research.google.com/)

**Learn more about [CUDA-Q](https://developer.nvidia.com/cuda-q) with NVIDIA official [GitHub](https://github.com/NVIDIA/cuda-quantum/). Running the tutorials in the CUDA-Q container (download from [NGC](https://catalog.ngc.nvidia.com/)) with the corresponding version `X.X.X` or `latest` is highly recommended. Please follow the [instruction guide](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/quantum/containers/cuda-quantum).**
<br>
<br>
<br>
*Follow the steps below to run cudaq tutorials with free T4 GPU backend
<br>
<br>
<img src="https://github.com/user-attachments/assets/8427fd9c-67ac-44db-ae65-321e914308f0" width="800">
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
```
Squirtle007/CUDA-Q
```

**Then scroll down and click on the Colab tutorials with the desired version (ex. `0.7.1`)**
<img src="https://github.com/Squirtle007/CUDA-Q/assets/66664309/fc80dd75-ab8f-45f9-88f3-0b1dd6cb6b3e" width="800">
<br>
<br>
<br>

**Step 3. Make sure to select `Edit > Notebook settings > T4 GPU` as the backend for acceleration**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA-Q/assets/66664309/9d804b43-e56b-489f-a267-395411ed014c" width="800">
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA-Q/assets/66664309/d00f3c60-960b-4ad1-a7d5-fc55d48e4fb4" width="450">
<br>
<br>
<br>

**Step 4. Run the commands at the very beginning to set up CUDA-Q in the Colab environment.**
<br>
<br>
Version `0.8.0` as an example:
```
%pip install cuda-quantum==0.8.0
```
  
Starting from v0.9.0, the package has been renamed to **cudaq**: 
```
%pip install cudaq==0.9.0
```
<br>
<br>
