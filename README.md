# Tutorial_Enviroment_Buildup
## This tutorial is about how to setup a new environment with correct version of python, pytorch, cuda, conda, etc.


  
Step 1: install conda

  Go to [Anaconda website](https://www.anaconda.com/distribution/)
  
  Linux - python 3.6 -download Anaconda-XX-xxx.sh file
  
    In local home, bash Anaconda-XX-xxx.sh file to install.
    Add the commands in .bashrc file.
    source .bashrc
  
  
Step 2: build enviroment

    conda create -n your_env_name python=3.6
  
Step 3:

    source activate your_env_name
  
## Mannually install pakages  
Step 4: install pytorch

    conda install pytorch=0.4.1 cuda90 -c pytorch
 https://pytorch.org/get-started/previous-versions/
    
Step 5:
    pip install other packages such as matplotlib, torchvision,....

## Use requirement.txt to install packages
    pip install -r requirement.txt
  
  

## Other commands:

Visualize Conda enviroments:

    conda info --envs
    
    
Pytorch version:

    python
    import torch
    print(torch.__version__)
    
    
CUDA version:

    nvcc --version
    
Delete conda enviroment

    conda remove -n your_env_name --all

Duplicate an environment 
    
    conda create --name flowers --clone snowflakes

How To Use SSHFS to Mount Remote File Systems Over SSH
    sudo sshfs username@destination_address:/home/username/destination_folder local_folder/ -o allow_other
