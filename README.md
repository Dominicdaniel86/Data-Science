# Data Science Project

## How to Set Up This Project

**✅ Requirements**
Before starting, make sure you have installed:

- Python 3
- Anaconda (or Miniconda)

### Step 1 - Clone/Download the Project

```bash
git clone https://github.com/Dominicdaniel86/Data-Science.git
cd Data-Science
```

### Step 2 - Create the Conda Environment

Run this command in the project root folder (where `environment.yml` is located):

```bash
conda env create -f environment.yml
```

This will install all required dependencies automatically.

### Step 3 - Activate the Environment

```bash
conda activate data-science
```

(*The environment name needs to match the name defined inside `environment.yml`.*)

### Step 4 - Run the Project

```bash
python main.py
```

### (Optional) Step 5 - Deactivate the Environment

When you're done working:

```bash
conda deactivate
```

### How to Update the Dependencies

Whenever you update your Anaconda environment using `pip` commands like this:

```bash
pip install numpy
```

make sure to also add the dependency to the `environment.yml` file. This ensures a consistent environment for all other project members.

### How to Load Updated Dependencies

If someone updates the `environment.yml` file, run this command:

```bash
conda env update -f environment.yml --prune
```

This updates your environment safely.
