### Computer

Participants must work on a computer with a Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) on which they have administrative privileges. 

### Software

To participate in this workshop, you will need to prepare the following:

- Install Shell and Git.
- Create a GitHub account.
- Set up an SSH connection to GitHub. 
  
Please refer to [this page](https://carpentries-incubator.github.io/collaborative-git-and-github-lesson/) for detailed instructions.

- Install Miniconda. Please refer to [this page](https://coderefinery.github.io/installation/conda/) for instructions.
- Create a Conda environment for the workshop. Please refer to [this page](https://coderefinery.github.io/installation/conda-environment/) for instructions.

#### Conda
```
conda --version
```
returning (something similar to):
```
conda 22.9.0
```

#### Conda environment for the workshop
```
conda activate coderefinery
python -c "import sys; assert sys.version_info.major>=3"
jupyter-lab --version
pytest --version
sphinx-build --version
snakemake --version
conda deactivate
```
returning (something similar to):
```
3.9.10
pytest 7.0.1
sphinx-build 4.4.0
7.1.1
```

#### If something does not work:
Follow the corresponding setup instructions. If you still need help, come to our dedicated setup session.

