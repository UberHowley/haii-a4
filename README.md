# Assignment #4 Setup Instructions

## Step #0 Create a Discord Account, Server, and Bot
Read the instructions in Glow and watch the Assignment 4 video for directions on how to do this.

## Step #1 Install Necessary Programming Modules (new!)
This week, in addition to Anaconda Python 3.8 (or greater) with Jupyter Notebooks and pandas, you'll also need to install the `discord`, `fastai`, and `nest_asyncio` modules. 

For discord.py, we'll need the following lines of code in terminal:
```
conda config --add channels conda-forge
conda config --set channel_priority strict
conda install discord.py
```

For fastai, we should use conda (and on Windows, the conda shell), as we're using Anaconda python:

```
conda install -c fastai -c pytorch -c anaconda fastai gh anaconda
```
(If you pip install fastai, you'll need to install `pytorch` first, [according to the fastai installation instructions](https://docs.fast.ai/#Installing))

`nest_asyncio` is needed for running discord.py code in Jupyter notebooks. You should be able to install it with:

```
conda install conda-forge::nest-asyncio`
```

If any of these conda installs fail, you should be able to force install them directly in the Jupyter notebooks with:
```
!pip install fastai
!pip install nest_asyncio
!pip install discord
```

### Using Anaconda
Install Anaconda Python 3.8 (or greater) if you haven't already for our previous assignments. [https://www.anaconda.com/distribution/](https://www.anaconda.com/distribution/) You'll need Jupyter Notebook, and pandas, at the very least.

### Problems with Module Versions, or with Windows machines
If you're using a Windows machine and the above installation instructions don't work, or encountering significant issues with module version and installation, consider using Google Colab to open up this assignment's Jupyter notebook. You can access any public GitHub Jupyter Notebook on Google Colab by replacing the github.com in the URL with colab.research.google.com/github, like so: `https://colab.research.google.com/github/UberHowley/haii-a4/blob/main/Satire_Bot.ipynb`. Make sure you save regularly! When you are reading data in our notebook, you need to copy the “data” folder to some place you can access from Colab. These instructions and more are available via the Video lecture for this assignment.


## Step #2 Download homework files
Download all the files in this repository. Place these files into a well-named folder on your computer, and click on the zip file to unzip the data folder. You will zip all the files in this directory and submit the `.zip` file to Glow when completed.

## Step #3 Open the Jupyter Notebook

### Opening Notebooks: VS Code Option
If you have VS Code, it has built-in support for running Jupyter Notebooks. You'll be prompted to select a Python environment, and should choose the anaconda python environment so you don't have to separately install scikit-learn, pandas, numpy, etc. individually.

### Opening Notebooks: Terminal Option
In your terminal, navigate to your homework folder and run `jupyter notebook .` to start the notebook. A notebook session should open up in your browser.

On a Mac, you can run a Jupyter notebook from Terminal by typing `jupyter notebook name_of_file_here.ipynb`. On Windows, you will do [something similar](https://pythonforundergradengineers.com/opening-a-jupyter-notebook-on-windows.html) but by running the 'Anaconda Prompt' that comes with the Anaconda distribution.

### Opening Notebooks: Anaconda Graphical User Interface Option
Once Anaconda is installed on your machine, open an application called Anaconda-Navigator. On the main page, click the 'launch' button on the Jupyter Notebook tile. A notebook session should open up in your browser.

### Opening Notebooks: Google Colab Option
If you lack space on your machine for installing libraries, Google Colab can be a good option. Google Colab is a cloud-based Jupyter Notebook. Instructions for using Google Colab for this assignment are available on the assignment page.

## Step #4
Once you have the Jupyter Notebook for this assignment open, then follow the instructions described therein. 

# Jupyter Notebooks
If you haven't used Jupyter Notebooks before, a good first step for you would be to read the [Jupyter Notebook Tutorial: The Definitive Guide](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook) and take the User Interface Tour in the Jupyter notebook Help menu once you've opened your first Jupyter Notebook.

# Resources
- General resources: 
    * [Jupyter Notebook Tutorial: The Definitive Guide](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook)
    * [Python3 Documentation](https://docs.python.org/3/index.html) (tutorial and library reference are likely useful)
    * Python tutorials from [w3schools](https://www.w3schools.com/python/) and [Scrimba](https://scrimba.com/learn/python).
    * [Python pandas documentation](https://pandas.pydata.org/pandas-docs/stable/)
    * [A list of python pandas tutorials](https://pandas.pydata.org/pandas-docs/stable/getting_started/tutorials.html)
    * [pandas.series.str.count](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.str.count.html)
- Fastai:
  * [fastai Language Modeling](https://docs.fast.ai/tutorial.text.html#The-ULMFiT-approach)
  * [fastai help forum](https://forums.fast.ai/)
  * [fastai](https://www.fast.ai/)
- discord.py:
  * [Discord Bot Account](https://discordpy.readthedocs.io/en/stable/discord.html)
  * [discord.py Documentation](https://discordpy.readthedocs.io/en/stable/index.html#)
  * [discord.py Quickstart](https://discordpy.readthedocs.io/en/stable/quickstart.html)
