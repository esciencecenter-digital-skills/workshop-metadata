### Computer

Participants must work on a computer with a Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) on which they have administrative privileges.

### Software

To participate in this workshop, you will need to prepare the following (if you haven't already):
- Install Shell and Git. Please refer to [this page](https://coderefinery.github.io/installation/git-in-terminal/#installation)) for installation instructions.
- Create a GitLab account. [You can sign up here](https://gitlab.com/users/sign_up).
- Set up an SSH connection to GitLab (ED25519 preferred). Please refer to [this page](https://docs.gitlab.com/ee/user/ssh.html) for instructions.
- Install Miniconda. Please refer to [this page](https://coderefinery.github.io/installation/conda/) for instructions.
- Create a Conda environment for the workshop. Please refer to [this page](https://coderefinery.github.io/installation/conda-environment/) for instructions.

### To confirm that everything works

You should now be able to open [a terminal window](https://swcarpentry.github.io/shell-novice/#open-a-new-shell) and execute the following commands:

#### Git
```
git --version
```
returning (something similar to):
```
git version 2.37.1 (Apple Git-137.1)
```

#### GitLab account & SSH connection
```
ssh git@gitlab.com
```
returning (something similar to):
```
Welcome to GitLab, [username]!
Connection to gitlab.com closed.
```

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

