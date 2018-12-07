# Set up your computer
We recommend that you install Python through [Anaconda](https://www.anaconda.com/download). Choose "Python 3.7 version". 

Test your installation by running `python --version` in a terminal (in the "Anaconda Prompt" if you're on Windows). The output should contain "Python 3.7" and "Anaconda". 

After you've made sure that Anaconda is installed, go through the following steps: 
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
and try `conda activate elmed219` again. If that fails, use `source activate elmed219` instead.

### Install a Jupyter kernel
```bash
python -m ipykernel install --user --name elmed219 --display-name "ELMED219"
```

### Test your installation
Run through the notebook `0.0-test.ipynb`:
```bash
jupyter notebook
```
You can also use [JupyterLab](https://github.com/jupyterlab/jupyterlab): `jupyter lab`.

## Update
The code and environment will be updated throughout the course. Run the following two commands regularly:
* Update code: `git pull`
* Update environment: `conda env update`

# Troubleshooting