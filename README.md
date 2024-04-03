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

**Step 4. Search and select `CUDA Quantum` then specify compute resources and storage, etc**
<br>
<br>
![image](https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/935cc1b2-19d4-4e3e-8cb4-e41d2a40a7d9)
<br>
<br>
<br>

**Step 5. Click on the container (after initialization) to see more details and `launch` Jupyter Notebook**
<br>
<br>
![image](https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/14aed847-6301-4e7e-bb13-5e309cf107f4)
<br>
<br>
<br>


**Step 6. Within Jypyter Notebook open a `command window and` run the following commands to access built-in tutorials inside CUDA Quantum etc.**
<br>
<br>
![image](https://github.com/Squirtle007/CUDA_Quantum/assets/66664309/14aed847-6301-4e7e-bb13-5e309cf107f4)
<br>
<br>
```
sudo chown -R `stat . -c %u:%g` /home/cudaq/
cp -r /home/cudaq/ ~/cudaq
```


