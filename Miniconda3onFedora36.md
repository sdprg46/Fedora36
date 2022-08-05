# Miniconda3 on Fedora 36
To get set up and running with python on F36, I follow the following steps:

**1. First I download the latest version from the official repo:**
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

**2. Then I run the following to install Miniconda3:**
```
bash Miniconda3-latest-Linux-x86_64.sh
```

**3. I then accept the license agreement (by pressing _q_ to get to the end of it), and type _yes_ to initialize Miniconda3 when prompted.**

**4. The installation takes effect when the terminal is closed and reopened. The _base_ prefix appears at the beginning of the shell prompt. I don't want conda base environment to be activated by default, so I use:**
```
conda config --set auto_activate_base false
```

**5. For the change to take effect immediately, I then do:**
```
source ~/.bashrc
```

**6. To manually activate/deactivate the conda environment, I use the following commands:**
```
conda activate
conda deactivate
```

**7. To install the packages that I frequently work with, I use the following command:**
```
conda install numpy scipy sympy pandas matplotlib spyder jupyter
```

**8. I can then open a new jupyter notebook as follows:**
```
conda activate
jupyter-notebook
```
