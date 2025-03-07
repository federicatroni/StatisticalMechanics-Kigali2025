## Installing Python3

### 1. Anaconda Navigator
We will install Python3 via Anaconda Navigator.
To install Anaconda Navigator
Go here

[https://docs.anaconda.com/free/anaconda/install](https://docs.anaconda.com/free/anaconda/install)

Select your operating system by clicking one of

- Installing on Windows
- Installing on macOS

Select
"Download the Anaconda installer."


### 2. Create an environment for this course

We will use several Python packages.
We will bundle these into something called an "environment".

 Using **Anaconda Navigator**:
- Select "Environment" (on the left panel)
- Select "Create" 
- Name the environment `statmech_2025`
- Use the default python version

When the environment has been created

- Click the "play" button
(looks like a solid / filled right pointing arrowhead)
- Select "Open Terminal"
- When the terminal pops up, type the following commands one-by-one.

```
conda install numpy
conda install scipy
conda install matplotlib
conda install sympy
conda install pandas
```

Each `conda install` line may prompt you for a response. Answer `y` to all questions.


Or **from the terminal** type directly:

```
conda create --statmech_2025 python=3.9
conda activate statmech_2025
conda install numpy scipy matplotlib sympy pandas
```

To exit the environment type: `conda deactivate`
### 3. Install Anaconda applications

- Within Anaconda Navigator select "Home" (on the left panel)
- In the bar at the top, make sure it says
"All applications" on "statmech_2025"
- Find the JupyterLab application, select "Install"

### 4. Download/open files and start Jupyter Notebook

Either download the data from the github repository ([here](https://github.com/federicatroni/StatisticalMechanics-Kigali2025.git)'s the link) or copy it from the pen drive. Then follow these instructions:
#### 1. Activate Your Conda Environment (if using Conda)

If you're using Conda, first activate the environment where Jupyter is installed:

```bash
conda activate my_env
```
Replace `my_env` with your environment name.

#### 2. Launch Jupyter Notebook

Once in the correct environment, start Jupyter Notebook by running:

```bash
jupyter notebook
```
This will open a Jupyter interface in your default web browser.

### Using Anaconda Navigator

1. Open **Anaconda Navigator** (search for it in the Windows Start Menu).
2. Click **"Launch"** under Jupyter Notebook.

### Using Command Prompt or PowerShell (better for MacOS users)

1. Open **Command Prompt (cmd)** or **PowerShell** (`Win + R`, type `cmd` or `powershell`, and hit Enter).
2. Navigate to your desired working directory:
   
   ```bash
   cd path\to\your\folder
   ```

3. Run:
   
   ```bash
   jupyter notebook
   ```

### Using Windows Start Menu

If Jupyter Notebook is installed system-wide, you can also search for **"Jupyter Notebook"** in the Windows Start Menu and open it directly.
