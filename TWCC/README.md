# Running CUDA-Q on Taiwan Computing Cloud (TWCC)

Learn more about [CUDA-Q](https://developer.nvidia.com/cuda-q) with NVIDIA's official [GitHub repository](https://github.com/NVIDIA/cuda-quantum/). We recommend using the CUDA-Q container with tag `latest` for these tutorials. Please follow the [instruction guide](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/quantum/containers/cuda-quantum) (Docker required).

## Setup Instructions

### Step 1: Sign up for TWCC
Visit [TWCC](https://www.twcc.ai/) and create an account.

<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/225641a3-c7ad-4547-86c3-f1ecdbf308f3" width="800">

### Step 2: Navigate to Interactive Container
Log in and go to `Interactive Container` on the dashboard.

<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/03a3c1ed-1387-4ba1-be50-65e0983e76c7" width="800">

### Step 3: Create a New Container
Select `CREATE` to set up a new container.

<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/6a647a07-7a48-41a7-97b8-efee2c0a5dc2" width="800">

### Step 4: Configure CUDA Quantum Container
Search and select `CUDA Quantum`, then specify compute resources and storage requirements.

<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/935cc1b2-19d4-4e3e-8cb4-e41d2a40a7d9" width="800">

### Step 5: Specify Resources
Configure compute resources and storage. For example, select 1 GPU, then review and create the container.

<img src="https://github.com/user-attachments/assets/b31153fd-f02c-43c4-9fad-9263d39c6d97" width="800">

### Step 6: Launch Jupyter Notebook
Click on the container (after initialization) to see details and launch Jupyter Notebook.

<img src="https://github.com/user-attachments/assets/3b313ab3-aac8-45a2-be19-c6158111f5bf" width="800">

<img src="https://github.com/user-attachments/assets/506513e8-8c58-4689-a3cd-cd65d8ee7901" width="800">

### Step 7: Setup CUDA-Q Tutorials
Open a `Terminal` in Jupyter Notebook and run the following commands to access built-in tutorials and install necessary libraries:

<img src="https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/b7fe4abb-8c91-4655-941f-e55a5230c7d7" width="600">

```bash
sudo chown -R `stat . -c %u:%g` /home/cudaq/
rm -rf ~/cudaq
cp -r /home/cudaq/ ~/cudaq
sudo apt update && sudo apt install -y libgfortran5
```

### Step 8: Access Additional Tutorials
To access additional tutorials from this repository, use:

```bash
git clone https://github.com/Squirtle007/CUDA_Q.git
```

## Next Steps
Navigate to the `CUDA-Q/TWCC/latest` folder and explore the tutorials to get started with quantum programming using CUDA-Q 🚀
