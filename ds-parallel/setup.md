### Requirements

- A programming editor, when in doubt we recommend [Microsoft VS Code](https://code.visualstudio.com/).
- Python version 3.11 or newer, we recommend [uv](https://docs.astral.sh/uv/), or [Anaconda](https://www.anaconda.com/products/individual) / 
  [Miniconda](https://docs.conda.io/en/latest/miniconda.html) to set up Python.
- Git. If you're on Windows, follow these instructions: [Git for Windows](https://carpentries.github.io/workshop-template/#shell).
- Graphviz. Follow these instructions: [Installing Graphviz](https://graphviz.org/download/)

**Data used in this course:**
- New York taxi data ([description](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)). The instructions
below help you download the data.

To follow along with the workshop, you need to prepare an environment. Clone the workshop repository
that we prepared:

```bash
git clone https://github.com/esciencecenter-digital-skills/parallel-python-workshop.git
cd parallel-python-workshop
```

You may prepare the environment either in `conda` or using `uv`:

### UV

UV is our recommended tool to manage the Python environment. Please follow the [UV install instructions](https://docs.astral.sh/uv/#installation) if you haven't already. Then, running from the directory where you cloned this repository, run the following commands:

```bash
uv sync
uv run ny-taxi/download.py
uv run pytest
```

### Conda

If you want to use Conda instead of UV, you can do the following:

```bash
conda env create -f environment.yml
conda activate parallel-python
python ny-taxi/download.py
pytest
```

If the tests pass, you're all good! Otherwise, please contact us before the workshop.
