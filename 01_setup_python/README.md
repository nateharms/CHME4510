# How to install Python and start up `jupyter` notebooks.

## What is Python?

### The asnwer, from `python.org`

> Python is an interpreted, object-oriented, high-level programming language with dynamic semantics. Its high-level built in data structures, combined with dynamic typing and dynamic binding, make it very attractive for Rapid Application Development, as well as for use as a scripting or glue language to connect existing components together. Python's simple, easy to learn syntax emphasizes readability and therefore reduces the cost of program maintenance. Python supports modules and packages, which encourages program modularity and code reuse. The Python interpreter and the extensive standard library are available in source or binary form without charge for all major platforms, and can be freely distributed.

### Why are we using Python?

Python is one of the most widely used coding languages with thousands of useful softwares (or packages) based on the Python programming language. Part of the reason why it is a popular choice for engineers is large collection of online users and because of powerful analysis packages such as `numpy`, `scipy`, and `matplotlib` (which will be used in this course). These tools will allow us to work with large amounts of reactor data, solve ODEs, plot the results, and generate models for reactors.

### What is `jupyter` and why are we using it? 

Jupyter (pronounced like the planet) is a web application that allows users to run and visualize code. It easily allows for users to write code and text, perform calculations, generate plots, and save the results as PDF, python (`.py`), Jupyter (`.ipynb`) or HTML formats. We will be using this when writing code, generating plots, and doing excercises. 

## How to install Python?

### 1) Download and set-up Anaconda

First, save the `environment.yml` file to your computer. Next, download the graphical installation of Anaconda from [this link](https://www.anaconda.com/products/individual). Anaconda is an easy way to install Python, Jupyter and many other packages easily. Follow the on-screen prompts when setting up Anaconda. If you have any questions, the following video is a good tutorial.

[![](http://img.youtube.com/vi/LrMOrMb8-3s/0.jpg)](http://www.youtube.com/watch?v=LrMOrMb8-3s "Anaconda Tutorial")

### 2) Set-up your Conda Environment

Once Anaconda is installed, fire up the Anaconda Navigators and go to the `Enviornments` tab. An environment is a collection of python codes or packages that all work together in a specific way. For example, you could have one environment that is used for a specific project with specific packages installed and you could have another for a different project. For this class, we will be using a single environment. 

In the `Environments` tab, click the `Import` button and specify the path to the `environment.yml` file you downloaded a little while ago. This will prompt Anaconda to create an environment titled `chme4510`.

### 3) Setting your Jupyter Kernel

Navegate back to the `Home` tab and launch `Jupyter Notebook`. Install `Jupyter` if it hasn't been installed yet. This will take you to your web browser with Jupyter running in it. On the top menus on the very right, click `New` and go down to `Terminal`, this will launch a terminal in your browser (don't worry, we're only doing this once).

Copy and paste the following command into your terminal in your browser and press enter to run it.

`source activate chme4510 && python -m ipykernel install --user --name myenv --display-name "Python (chme4510)"`

This command is settign your kernel (or connection) between Jupyter and the environment you made allowing you to use your installed packages in your Jupyter Notebooks.

Next, close the browser running the terminal and return to the web browser running Jupyter. In the browser running Jupyter, refresh the page.

### 4) Creating Jupyter Notebooks

Feel free to navegate to any location in your computer using the web browser running Jupyter. To create a notebook in this location, click the `New` tab and select the `Python (chme4510)` option to create a new notebook. 

In this notebook you can enter variables, run cells (smaller blocks of code), and practice coding throughout the remainder of this course. To run code or cells, either click the Play button at the top or hold `Shift+Enter` together. 

