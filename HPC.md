# HPC Commands



## Useful commands


resource allocation
    
```bash

srun -A vxc204_aisc -p aisc -c 24 --gres=gpu:1 --mem=64G --time=9:50:00 --pty bash

```

```bash