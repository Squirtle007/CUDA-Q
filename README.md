# Runing CUDA-Q in TWCC environment


**Step 1. Sign up [TWCC](https://www.twcc.ai/)**
<br>
<br>
![image](https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/225641a3-c7ad-4547-86c3-f1ecdbf308f3)
<br>
<br>
<br>

**Step 2. Log in and navigate to `Interactive Container` on the dashboard**
<br>
<br>
![image](https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/03a3c1ed-1387-4ba1-be50-65e0983e76c7)
<br>
<br>
<br>


```
sudo chown -R `stat . -c %u:%g` /home/cudaq/
cp -r /home/cudaq/ ~/cudaq
```
