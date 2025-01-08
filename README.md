# Common Research

* Python
* Git
* SSH 

- The best reference and starting point for using the HPC is the [Case HPC Website](https://sites.google.com/a/case.edu/hpcc/).
- HPC resource management guid is available [here](https://cwru-llm-workshop.notion.site/HPC-Resources-1056ed3cae46806cbc1cd8b32ab1cb17).

## Research on LLMs

Notes:
- Make sure to read [Dr. Han](https://ahxt.github.io/)'s [How to be a Good HPC Citizen](https://mlcase.notion.site/How-to-be-a-Good-HPC-Citizen-160867616eb980fa8c76c3965d729a7b) notes.
- All pretrained weights are available on `/mnt/rds/VipinRDS/VipinRDS/users/mxh1029/llms/hub` directory on the HPC as read-only files. You don’t need to download the model weights.
- For inference tasks, you can directly use the pretrained weights.
- For tasks that require modifying the weights (e.g., fine-tuning), you must save the weights in your own directory.
