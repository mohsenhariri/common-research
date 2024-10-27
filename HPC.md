# HPC Commands



## Set HPC ENVs

**~** means the home directory of the user `/home/username`

```bash

copy this to your `~/.bashrc` file
    
```bash
export XDG_CACHE_HOME=/your/path/to/cache
```

```bash
source ~/.bashrc
```

verfiy the path is set correctly

```bash
echo $XDG_CACHE_HOME
```


## Useful commands





resource allocation
    
```bash

srun -A vxc204_aisc -p aisc -c 24 --gres=gpu:1 --mem=64G --time=9:50:00 --pty bash

```



## Conda Environment


* install conda
* first download the latest version of miniconda from  https://docs.anaconda.com/miniconda/
copy the link from Miniconda3 Linux 64-bit (bash installer) to download the latest version of miniconda

for example:
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

then run the bash script to install miniconda

```bash


* https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html

go to this link ot find the latest version of miniconda


```

check Conda envs

```bash
conda env list
```

create a new conda environment


```bash
conda create --name env_name python=3.12.3
```

activate the conda environment

```bash
conda activate env_name
```

install packages



remove env completely

```bash
conda remove --name env_name --all
```

update conda base

```bash

conda update -n base -c defaults conda
```

