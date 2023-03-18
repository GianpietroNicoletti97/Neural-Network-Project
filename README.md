# NNDL

### Setting up a local repository

The following instructions need to be followed any time a new local repository is created. If you are working in a location where such repo already exists, what follows doesn't need to be repeated every time.

Generate your Token on GitHub following this [guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token). Copy the token to a safe place. Remember you can see it only the first time, otherwise if you lose it you have to create another one.

   * Clone your repository (i.e. create a local repository cloned from your remote repository)

   `git clone https://<YourToken>@github.com/GianpietroNicoletti97/NNDL.git`

   where <YourUsername> it your GitHub username and <YourToken> is the token as copied from the GitHub webpage. A new directory will appear in your current directory. Get into it:

   `cd NNDL/`

   * Configure your username and email:

   `git config --global user.name "<YourUsername>"`

   `git config --global user.email "<YourEmail>"`


### Requirements

* PyTorch: version 1.13.0, package for Conda, Cuda 11.6 or CPU 

	* GPU: `conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia`
	* CPU: `conda install pytorch torchvision torchaudio cpuonly -c pytorch`

* torch-sparse 0.6.15: `pip install torch-sparse`

* PyTorch Geometric: `pip install torch-geometric`
	
__ONLY FOR WINDOWS USER__

Notice that, in this case, install it __directly from "anaconda prompt"__ and not using the command `!pip...` in the notebook
