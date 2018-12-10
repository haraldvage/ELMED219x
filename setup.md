# Set up your computer

## Anaconda
We recommend that you install Python using the [Anaconda Distribution](https://www.anaconda.com/download). Make sure to choose the "Python 3.7 version. We'll use the Conda Package Management System that comes with the Anaconda Distribution. From the [documentation](https://conda.io/docs):
> Conda is an open source package management system and environment management system that runs on Windows, macOS and Linux. Conda quickly installs, runs and updates packages and their dependencies. Conda easily creates, saves, loads and switches between environments on your local computer. 

After installation, run `python --version` in a terminal (in the "Anaconda Prompt" if you're on Windows). If the output contains "Python 3.7" and "Anaconda" you should be all set for the next steps.

## GitHub
The code for the course is hosted on the code sharing platform GitHub (where you're reading this). If you haven't already signed up for a GitHub account please do so now. We also recommend using the platform for your own projects throughout the course. https://github.com/join.

## Kaggle
[Kaggle](https://www.kaggle.com) is an online community of data scientists hosting a large collection of data sets and data science competitions. It's the source for several of the data sets used in the course. The course project will be hosted on Kaggle. Create an account here: https://www.kaggle.com. 

## Get ready for the course

After you've made sure that Anaconda and Git are installed, go through the following steps: 
### Download the repository: 
```bash
git clone https://github.com/MMIV-ML/ELMED219x
cd ELMED219x
```
### Configure the Python environment
```bash
conda env update
```

### Activate environment:
```bash
conda activate elmed219
```
If you're using Linux or MacOS and the above command fails, run 
```bash 
source ~/.bash_profile
``` 
and try `conda activate elmed219` again. If that fails, activate the environment by writing `source activate elmed219` instead.

### Install a Jupyter kernel
```bash
python -m ipykernel install --user --name elmed219 --display-name "ELMED219"
```

### Test your installation
Run through the notebook `0.0-test.ipynb` in the `notebooks` folder:
```bash
cd notebooks
jupyter notebook
```
Instead of Jupyter Notebook you can use [JupyterLab](https://github.com/jupyterlab/jupyterlab): `jupyter lab`.

## Update
The code and environment will be updated throughout the course. Run the following two commands regularly:
* Update code: `git pull`
* Update environment: 
```bash
conda activate elmed219
conda env update
```

# Troubleshooting