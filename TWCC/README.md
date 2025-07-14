# Running CUDA-Q on Taiwan Computing Clond (TWCC)

**Learn more about [CUDA-Q](https://developer.nvidia.com/cuda-q) with NVIDIA official [GitHub](https://github.com/NVIDIA/cuda-quantum/). Running the tutorials in the CUDA-Q container with the tag `0.6.0` is highly recommended. Please follow the [instruction guide](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/quantum/containers/cuda-quantum) (Docker required).**
<br>
<br>
<br>
*Follow the steps below to set up CUDA-Q on TWCC:
<br>
<br>
**Step 1. Sign up [TWCC](https://www.twcc.ai/)**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/225641a3-c7ad-4547-86c3-f1ecdbf308f3" width="800">
<br>
<br>
<br>

**Step 2. Log in and navigate to `Interactive Container` on the dashboard**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/03a3c1ed-1387-4ba1-be50-65e0983e76c7" width="800"><br>
<br>
<br>

**Step 3. Select `CREATE` to set up a container**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/6a647a07-7a48-41a7-97b8-efee2c0a5dc2" width="800"><br>
<br>
<br>
<br>

**Step 4. Search and select `CUDA Quantum` then specify compute resources and storage, etc**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/935cc1b2-19d4-4e3e-8cb4-e41d2a40a7d9" width="800"><br>
<br>
<br>
<br>

**Step 6. Specify compute resources, storage, etc. For example, using 1 GPU, then review/create the container:**
<br>
<br>
<img src="https://github.com/user-attachments/assets/b31153fd-f02c-43c4-9fad-9263d39c6d97" width="800"><br>
<br>
<br>
<br>

**Step 5. Click on the container (after initialization) to see more details and `LAUNCH` Jupyter Notebook**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/14aed847-6301-4e7e-bb13-5e309cf107f4" width="800"><br>
<br>
<br>
<br>

**Step 6. Within Jypyter Notebook open a `Terminal` and run the following commands to access built-in tutorials inside CUDA Quantum**
<br>
<br>
<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/b7fe4abb-8c91-4655-941f-e55a5230c7d7" width="600"><br>
```
sudo chown -R `stat . -c %u:%g` /home/cudaq/
cp -r /home/cudaq/ ~/cudaq
```
<br>
<br>
<br>

**Step 7. To access additional tutorials in this repository, use the following `git clone` command**
```
git clone https://github.com/Squirtle007/CUDA_Quantum.git
```
<br>
<br>

