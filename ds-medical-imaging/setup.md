# Setup

## Installing the Python Environment

We'll use [Mamba](https://mamba.readthedocs.io/en/latest/index.html) (a faster alternative to [Conda](https://docs.conda.io/en/latest/) fully compatible with it) to set up the Python environment. [The environment YML file](https://github.com/esciencecenter-digital-skills/medical-image-processing/blob/main/learners/environment.yml) for the lesson is available on GitHub.

### Installing Mamba via Miniforge

Miniforge is a minimal installer for Conda that includes Mamba. Here are the installation instructions for different operating systems:

:::::::::::::::: spoiler

#### Windows
1. Download the Miniforge3 installer for Windows [from the official GitHub repository](https://github.com/conda-forge/miniforge?tab=readme-ov-file#miniforge3).
2. Run the installer and follow the prompts.

::::::::::::::::::::::::

:::::::::::::::: spoiler

#### macOS and Linux

1. Open a terminal window.
2. Download the installer using `curl` or `wget` or your favorite program and run:
```bash
curl -L -O "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash Miniforge3-$(uname)-$(uname -m).sh
```
or
```bash
wget "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash Miniforge3-$(uname)-$(uname -m).sh
```
3. Follow the prompts to complete the installation.
4. Close and reopen your terminal to apply the changes.

::::::::::::::::::::::::

If you encounter any issues, please refer to the [official Mamba documentation](https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html).

If you're unable to install Mamba, you can alternatively [install Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) as a fallback option. If you choose this route, remember to replace `mamba` with `conda` in all subsequent commands in these instructions.

After you have a working Mamba (or Conda) installation you can proceed to create and activate the environment.

### Creating the Environment

1. Open your terminal:
   - On Windows: Open "Miniforge Prompt" or "Command Prompt".
   - On macOS/Linux: Open your regular terminal.
2. Navigate to your lesson workspace directory.
3. Run the following command:

```bash
mamba env create -f https://raw.githubusercontent.com/esciencecenter-digital-skills/medical-image-processing/main/learners/environment.yml
```

4. Wait for the installation to complete. This may take a few minutes.

### Activating the Environment

After the installation is complete, activate the environment:

```bash
mamba activate medical_image_proc
```

## Downloading Image Files from Zenodo

Now that you have the environment set up, let's download the necessary files from Zenodo.

### Option A: Manual Download

1. Open your web browser and navigate to [this lesson's data Zenodo record address](https://zenodo.org/records/13311246).
2. Look for the "Files" section on the page.
3. Click tha download button for downloading the `data.zip` file containing the images.
4. Once downloaded, extract the contents of the ZIP file.
5. Move the extracted folder to your lesson workspace directory (where you'll create notebooks and work during the lesson).

### Option B: Using Zenodo API

You can use the Zenodo API to download the files. The `zenodo_get` package should already be installed in your environment.

1. Ensure you're in your lesson workspace directory and your `medical_image_proc` environment is activated.
2. Use the following command in your terminal (Miniforge Prompt if you are a Windows user):
```bash
zenodo_get 13311246
```
3. Extract the contents of `data.zip`.

Remember to keep the `medical_image_proc` environment activated throughout the entire lesson. If you close your terminal or restart your computer, you'll need to activate the environment again using the activation command above.

Also, remember to verify that the extracted folder is in your lesson workspace directory (where you'll create notebooks and work during the lesson).
