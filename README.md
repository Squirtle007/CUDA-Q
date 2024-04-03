# Runing CUDA-Q in TWCC environment


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


```
sudo chown -R `stat . -c %u:%g` /home/cudaq/
cp -r /home/cudaq/ ~/cudaq
```
