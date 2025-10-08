# python-template

A dev environment template for students of courses by the ML working group.

## Tutorial

This tutorial will guide you through setting up a local development environment for your machine learning courses.

If you prefer to not work on your local machine, you can also use services like [Google Colab](https://colab.research.google.com/).

We will use [VSCode](https://code.visualstudio.com/) as the IDE and [uv](https://docs.astral.sh/uv/) as the package manager.
Feel free to use any other package manager, but we recommend using uv for its simplicity and environment management features.
To follow this tutorial, you should have git, VSCode, and uv installed on your machine.

### 1. Clone the repository and open it in VSCode

- Navigate to a folder where you want to store the code.

- Clone the repository using the command:

  ```bash
    git clone https://github.com/ml-uhh/lecture-dev-template.git
  ```

- Open the folder in VSCode.

  ```bash
    code lecture-dev-template
  ```

### 2. Setup VSCode for use with Jupyter notebooks and Python

- Install the [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) extension
- Install the [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) extension

### 3. Setup the Python environment

We have already initialized the project. Use `uv` to install the dependencies and create an environment.

```bash
  uv sync
```

There should now be a new folder containing the environment at `./.venv/`

### 4. Open a notebook

- Open the [numpy tutorial notebook](tutorials/introduction_numpy.ipynb).
- In the top right corner, select the Python environment created by `uv` (should be called `lecture-dev-template`).
- You should now be able to run the notebook cells.

### 5. Add more packages

You may notice that some cells report missing packages. For example, `numpy` and `matplotlib` are missing.
You can add them using `uv`:

```bash
  uv add numpy matplotlib
```
