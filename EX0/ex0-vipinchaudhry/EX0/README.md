# Homework 0
**Introduction to Data Science - CITHN1007**  
*This should be completed by the first exercise session.*  


Welcome to the Data Science course at TUM Heilbronn. In this class, we will be using a variety of tools that will require some initial configuration. To ensure everything goes smoothly moving forward, we will set up the majority of those tools in this homework. This homework will not be graded, but **it is essential that you complete it before the first exercise** as it sets up the tools that we will be using in class for exercises.

## 1. Setup

We'll often work on practical skills related to data science. That means we'll write code, and we'll do that in a programming language called Python.

Python has three advantages for this class: it's pretty easy to learn, it's the language of choice for many data scientists, and it can be used inside of Jupyter Notebooks – more on the latter will follow later.

We also assume that you know the basics of how to work with a terminal / console. If you don't check out an introduction like [this](http://tutorial.djangogirls.org/en/intro_to_command_line/).  

First, we'll need to install some things:

### 1.1 Installing Python

Chances are, if you're on a Linux machine or Mac, you already have Python installed. You can simply try to run python from a console by running

```
$ python
```

However, as most software, Python comes in different versions and is packaged differently depending on your needs. In this class we'll use a Python distribution called Anaconda. Anaconda comes with a lot of packages that we'll need, so it is the most hassle-free option for us.

Anaconda is both a package manager and an environment manager. A package manager manages, well, packages. Packages add specific pieces of functionality - there are packages for web scraping, or for data visualization, for example. An environment manager, in contrast, allows you to have different versions of packages installed at the same time. We'll dive into environments and packages when we need them at a later point.

Anaconda comes in two flavors: the "full" Anaconda distribution and Miniconda. The full distribution comes with a ton of pre-installed packages and a bit of other bloat (i.e. a desktop application), while Miniconda is more lightweight and contains only Python and Conda. I tend to have a seperate environment for every project so I personally prefer Miniconda, but the convienience of the full distribution may be nicer starting out. 

Go to [this website](https://www.anaconda.com/download/success) and install anaconda for Python 3.12 for your operating system. [Here](https://docs.continuum.io/anaconda/install) are installation instructions if you need them. If you already have anaconda installed, please make sure that you're using the latest version or [update](http://docs.continuum.io/anaconda/install/update-version/) if necessary. For example, from a Bash shell (Linux or Mac) anaconda can be updated to the most recent version (2025.06-0) by entering commands in the command line. On Windows, the Anaconda installer also came with its own command line application, from which the same commands can be run:

```
$ conda update conda
$ conda install anaconda=2025.06-0
```



You'll have to create a new environment for Python 3.12 if you're not using that already. If you did a fresh install, this won't be necessary. Here is the update command:

```
$ conda install python=3.12
```

Once you've installed Anaconda, close your terminal window and re-open it - otherwise your terminal won't recognize the Anaconda commands.

Let's see whether Anaconda works as intended. Run:

```
$ conda --version
```

from your terminal. You should see something like this as a result:

```
$ conda --version
conda 23.7.4 
```

Similarly, for python, you should see something like this:

```
$ python --version
Python 3.11.5
```

You can also check out the [official website](http://conda.pydata.org/docs/test-drive.html) for more details on anaconda, environments, and packages.

### 1.2 Installing Jupyter Notebooks

***Check out the official Jupyter Notebooks documentation [here](http://jupyter.readthedocs.io/en/latest/index.html) for all the details***

We'll be running Python mostly through Jupyter Notebooks as they are great for the data science process and for teaching, but you should be aware of the other options we discuss here.

Notebooks make use of an improved, interactive client for python called [IPython](https://ipython.org/). IPython might already be installed in the latest version if you did a clean anaconda install. To check, we'll use anaconda to install the proper version of IPython. Run:

```
$ conda install ipython
```

Notebooks are stored in files that end with a `.ipynb` extension.
There is one included in this directory. Download it and save it to a folder.
Now, change directories in your console so that you're in the directory where the notebook file is saved and run:

```
$ jupyter notebook
```

This will start the notebook server and should open up a browser window point to [http://localhost:8888/](http://localhost:8888/) that will look like that:

![Jupyter Notebook Screenshot](jupyter.png)

Click on the `.ipynb` entry to see if it works. Now you're ready for the first exercise!

**Note**
Many IDEs and code editors (such as VS code) now support a Jupyter server within their own ecosystem. This may be preferable to the browser application for iPython, especially if you already have a favorite editing environment. 

### 2. Self Study: Python

I recommend that you go through [Google's Python Tutorial](https://developers.google.com/edu/python), sections Intro, Strings, Lists, Sorting, Dicts and Files. 
