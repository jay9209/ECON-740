# Econ 740

Matlab and Julia code repositories for ECON 777 class

## 1. Gresham codes 
The Matlab and Julia codes are based on [Cho and Kasa (2017, AER)](https://www.aeaweb.org/articles?id=10.1257/aer.20160665).

- `gresham4_matlab_function.m`
    - Matlab function script of gresham code
- `gresham4_matlab_parallel.m`
    - Parallel execustion code of `gresham4_matlab_function.m` using Octave on the **cluster**.
  
- `gresham4_julia_function.jl`
    - Julia function script translated from `gresham4_matlab_function.m`.
    - It is slightly modified to have parameters as inputs
- `gresham4_julia_local.jl`
    - Parallel execution code of `gresham4_julia_function.jl` on your **local** computer.
    - Adjust 'num_cores' depending on your CPU.
    - This code also generates some plots and histograms from the simulation results.
- `gresham4_julia_cluster.jl`
    - Parallel execustion code of `gresham4_julia_function.jl` on the **cluster**.
    - Can be executed using the shell file `gresham4_slurm.sh`.
- `gresham4_julia_slurm.sh`
    - Shell file that has to be executed on the **cluster** to run `gresham4_julia_cluster.jl`
- `gresham4_julia_gpu.jl`
    - GPU execustion code of `gresham4_julia_function.jl`.

## 2. Myerson codes
- `myerson8_matlab_local.m`
    - Local execution Matlab script of myerson code
- `myerson8_matlab_function.m`
    - Matlab function script of myerson code
- `myerson8_matlab_parallel.m`
    - Parallel execustion code of `myerson8_matlab_function.m` using Octave on the **cluster**.
- `myerson8_matlab_slurm.sh`
    - Shell file that has to be executed on the **cluster** to run `myerson8_matlab_parallel.m`
  
- `myerson8_julia_function.jl`
    - Julia function script translated from `myerson8_matlab_forparallel.m`.
    - It is slightly modified to have parameters as inputs
- `myerson8_julia_local.jl`
    - Parallel execution code of `myerson8_julia_function.jl` on your **local** computer.
    - Adjust 'num_cores' depending on your CPU.
- `myerson8_julia_cluster.jl`
    - Parallel execustion code of `myerson8_julia_function.jl` on the **cluster**.
    - Can be executed using the shell file `myerson8_slurm.sh`.
- `myerson8_julia_slurm.sh`
    - Shell file that has to be executed on the **cluster** to run `myerson8_julia_cluster.jl`

## 3. Compete codes
The Matlab and Julia codes are based on [this paper](https://github.com/jay9209/ECON-777/blob/main/Compete%20codes/competing13.pdf)
- `compete_matlab_pihat_benchmark.m`
    - Local execution Matlab script of compete (pihat model) code written by Kenneth Kasa.

- `compete_julia_pihat_benchmark.jl`
    - Local execution Julia script of compete (pihat model) code.
- `compete_julia_nopihat_benchmark.jl`
    - Local execution Julia script of compete (nopihat model) code.
- `compete_julia_pihat_cluster.jl`
    - Parallel execustion code of `compete_julia_pihat_benchmark.jl` on the **cluster**.
- `compete_julia_nopihat_cluster.jl`
    - Parallel execustion code of `compete_julia_nopihat_benchmark.jl` on the **cluster**.
- `compete_julia_slurm.sh`
    - Shell file that has to be executed on the **cluster** to run `compete_julia_pihat_cluster.jl`
- `compete_julia_pihat_gpu.jl`
    - GPU execustion code of `compete_julia_pihat_benchmark.jl`.