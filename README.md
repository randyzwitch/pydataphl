# PyData PHL Feb 2020: Introduction to using GPUs for Analytics

https://www.meetup.com/PyData-PHL/events/268253667/

In this talk, I highlighted the basic concepts of making Python code run faster, including the use of parallelization using GPUs. To help users replicate my environment, I created an environment.yml file to use with conda:

```shell
conda env create -f environment.yml
conda activate pydataphl
```

To run the GPU portion of this notebook, you need to use an NVIDIA GPU. I tried to make this work with Google Colab, but I couldn't get all of the packages to install properly. If someone figures this out, I'd happily accept a PR with the instructions.

### pydataphl_20200218.ipynb

This is the notebook that was presented during the actual meetup. In trying to make the data sizes accessible to any NVIDIA GPU a user might have, the relative performance improvements were directionally correct but not as impressive as if I had used larger data.

So if you were present at the meetup and want to see the original notebook, this it is, but the larger notebook is more impressive in terms of performance.

### pydataphl_20200219-larger.ipynb

This notebook shows the same relative comparisons, but with 256x more data (75MM vs. 295k). The performance improvements are much more in-line with what you would see in the real world when you keep the GPU saturated with data to process.
