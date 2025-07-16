# Running CUDA-Q on Google Colab

Learn more about [CUDA-Q](https://developer.nvidia.com/cuda-q) with NVIDIA's official [GitHub repository](https://github.com/NVIDIA/cuda-quantum/). Follow the steps below to run CUDA-Q with a free NVIDIA T4 GPU on Google Colab.

## Setup Instructions

### Step 1: Configure GPU Runtime
Ensure you select the T4 GPU backend for acceleration:
1. Go to `Edit > Notebook settings`
2. Select `T4 GPU` as the hardware accelerator

<img src="https://github.com/Squirtle007/CUDA-Q/assets/66664309/9d804b43-e56b-489f-a267-395411ed014c" width="800">

<img src="https://github.com/Squirtle007/CUDA-Q/assets/66664309/d00f3c60-960b-4ad1-a7d5-fc55d48e4fb4" width="450">

### Step 2: Install CUDA-Q
Install CUDA-Q via [PyPI](https://pypi.org/project/cudaq/) at the beginning of your notebook to set up the environment.

**For CUDA-Q version `0.11.0` as an example:**
```python
%pip install cudaq==0.11.0
```

**For versions earlier than `0.9.0`, use the package name `cuda-quantum`:**
```python
%pip install cuda-quantum==0.8.0
```

### Step 3: Verify Installation
Test your installation with a simple quantum circuit:

```python
import cudaq

@cudaq.kernel
def bell_state():
    qubits = cudaq.qvector(2)
    h(qubits[0])
    x.ctrl(qubits[0], qubits[1])

print(cudaq.sample(bell_state))
```

---

**Note**: For the most stable experience, running the tutorials in the CUDA-Q container is highly recommended. Please follow the [instruction guide from NGC](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/quantum/containers/cuda-quantum).
