# HPC Commands


## Set HPC ENVs

copy this to your `~/.bashrc` file
    
```bash
export XDG_CACHE_HOME=/your/path/to/cache
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
* make sure you're in an aisc node when you install conda

for example:
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

then run the bash script to install miniconda

And then run:

```bash
Miniconda3-latest-Linux-x86_64.sh
```
When prompted to provide the path to the conda installation, please create a new conda folder within your .cache

After the installation finishes, you should be able to run:
```bash
source ~/.bashrc
```
Then:
```bash
conda env list
```
And your conda environment should be displayed.


### create a new conda environment

```bash
