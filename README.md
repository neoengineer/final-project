# Final Project - BOIF509 (Spring 2020), Thomas May

## How to Explore This Project

### Work in Binder
- Currently running in Binder is not supported. The application requires a live video stream for iamge processing.

### Work in Colab
- Currently running in Colab is not supported. The application requires a live video stream for iamge processing.

### Work locally (requires local installation of [git](https://git-scm.com/) and [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html))
- Clone the repo using a shell (below) or [GitHub Desktop](https://desktop.github.com)

```sh
git clone https://github.com/neoengineer/final-project
cd final-project
jupyter lab
```
## Required Hardware

Jetson AGX Xavier series, Jetson TX2 series, Jetson TX1, or Jetson Nano, running Jetpack 4.3 
https://developer.nvidia.com/jetpack-43-archive


## Required packages

The packages used to run the code in the Binder instances are listed in [requirements.txt](requirements.txt) (Note that some of these exact version numbers may not be available on your platform: you may have to tweak them for your own use).

Edit the [requirements.txt](requirements.txt) file to meet the requirements of your project.

To install the requirements using [pip](http://conda.pydata.org), run the following at the command-line:

```sh
$ pip install --requirement requirements.txt
```

To install the requirements using [conda](http://conda.pydata.org), run the following at the command-line:

```sh
$ conda install --file requirements.txt
```

To create a stand-alone environment named ``final-project`` with Python 3.6 and all the required package versions, run the following:

```sh
$ conda create -n final-project python=3.6 --file requirements.txt
```

You can read more about using conda environments in the [Managing Environments](http://conda.pydata.org/docs/using/envs.html) section of the conda documentation.

## Git version control
To use git in a Binder instance, you have to set up your username and email as below:

```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

To avoid doing this every time you use Binder, include your username and email in the [git_setup.sh](git_setup.sh) file, which will be run via [postBuild](postBuild) immediately after building the Binder instance.


Every time you need to update the version of the [final-project.ipynb](final-project.ipynb) in your remote repo, run the following commands:

```sh
git add final-project.ipynb
git commit -m "Update final-project.ipynb"
git push
```

## License

The code in this repository is released under the [MIT license](LICENSE-CODE). Read more at the [Open Source Initiative](https://opensource.org/licenses/MIT).

