#### Code Editor

The recommended code editor for this lesson is Visual Studio Code, a popular code editor frequently used by researchers. You can download it from [the official website](https://code.visualstudio.com/). Follow the instructions on the website to install it on your operating system.

#### Setting up Codeium

1. Make sure you have an Integrated Development Environment (IDE) installed on your computer. Go to [the Codeium download page](https://codeium.com/download) to see a list of supported IDEs and installation instructions. Visual Studio Code is on the list, so if you followed the previous step, you are all set.

2. Open Extension Marketplace: Open the Extension Marketplace, which is the icon with boxes on the primary sidebar in your VS Code.

3. Install Codeium: Type Codeium in the marketplace search bar, open up the page and click the blue Install button.

4. Authorize: After installation is complete, you should be prompted by Visual Studio Code with a pop-up on the bottom right to authorize Codeium.
*If not, you should see an option to sign in to your Codeium account in the bottom left Accounts tab of your Visual Studio Code window.* 
Click the Sign in with Auth to use Codeium option. Either method (popup or Accounts tab) should redirect you to the Codeium website.

5. Create Account: If you do not have a Codeium account yet, you will be redirected to create an account.

6. Sign In: If you are not signed in, please sign in with your account details. Once you sign in, you will be redirected back to Visual Studio Code via pop-up.
Click Open Visual Studio Code, which should redirect you back to Visual Studio Code.
*If you are using a browser-based IDE, instead of being redirected back with pop-up, you will be routed to instructions on how to complete authentication by providing an access token. Please follow these instructions instead of Step 6, and then continue on with "Using Codeium."*

7. All Done! You will be asked to confirm the authentication in Visual Studio Code (click Open in the resulting pop-up).

#### Setting Up Your Python Environment

##### Installing Python

For the practical exercises in this lesson, we will use Python. If Python isn't already installed on your system, download it from the [official Python website](https://www.python.org/downloads/) and follow the provided instructions for installation.

##### Setting Up a Virtual Environment

To ensure a consistent and isolated Python environment, we recommend using a virtual environment. Virtual environments allow you to manage dependencies specific to each project without affecting other Python projects or your global Python setup.

Install [`virtualenv`](https://virtualenv.pypa.io/en/latest/installation.html) if it's not already available by running:

```bash
pip install virtualenv
```

Alternatively, you can use `pipx` to manage `virtualenv` installation:

```bash
pipx install virtualenv
```

Then, in your project directory, you can create a virtual environment:

```bash
python3 -m venv .venv
```

This command will create a `.venv` folder in your current directory to store all environment-specific files.

To activate the virtual environment, you will use the following command:

- On Windows, run `.venv\Scripts\activate.bat`
- On macOS/Linux, run `source .venv/bin/activate`

After activation, you should see the name of your environment (e.g., `.venv`) appear in your terminal prompt, indicating that the environment is active.

Once the environment is activated, you can install the packages needed for this lesson. Run the following command to install the necessary dependencies:

```bash
pip install -r https://raw.githubusercontent.com/olgaminaeva/gen-ai-coding/refs/heads/main/learners/files/requirements.txt
```

When you're finished with your work, after the end of this lesson, deactivate the virtual environment by typing `deactivate`. This will return you to your global Python environment.
