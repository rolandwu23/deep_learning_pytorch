# mlp_mnist_pytorch

# Dependencies

----

# Configure and Manage Your Environment with Anaconda

----

Per the Anaconda [docs](https://conda.io/projects/conda/en/latest/):

> Conda is an open source package management system and environment management system for installing multiple versions of  software packages and their dependencies and switching easily between them. It works on Linux, OS X and Windows, and was created for Python programs but can package and distribute any software.

# Overview

Using Anaconda consists of the following:

1. Install [`miniconda`](https://docs.conda.io/en/latest/miniconda.html) on your computer, by selecting the latest Python version for your operating system. If you already have `conda` or `miniconda` installed, you should be able to skip this step and move on to step 2.
2. Create and activate * a new `conda` [environment](https://conda.io/en/latest/using/envs.html).

* Each time you wish to work on any exercises, activate your `conda` environment!

# 1. Installation

**Download** the latest version of `miniconda` that matches your system.

|   | Linux	| Mac	 | Windows
--- | --- | --- | ---|
64-bit	| [64-bit (bash installer)](https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh)	| [64-bit (bash installer)](https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh)	| [64-bit (exe installer)](https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe)
32-bit	| [32-bit (bash installer)](https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh) |                         | [32-bit (exe installer)](https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe)

**Install** [miniconda](https://docs.conda.io/en/latest/miniconda.html) on your machine. Detailed instructions:

**Linux**: <http://conda.pydata.org/docs/install/quick.html#linux-miniconda-install>

**Mac**: <http://conda.pydata.org/docs/install/quick.html#os-x-miniconda-install>

**Windows**: <http://conda.pydata.org/docs/install/quick.html#windows-miniconda-install>

# 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work.

#### Git and version control

These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:

<pre> conda install git                                                                                                 
</pre>

#### Now, we're ready to create our local environment!

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
<pre>
git clone https://github.com/udacity/deep-learning-v2-pytorch.git
cd deep-learning-v2-pytorch
</pre>

2. Create (and activate) a new environment, named `deep-learning` with Python 3.6. If prompted to proceed with the install `(Proceed [y]/n)` type y.

**Linux** or **Mac**:
<pre>
conda create -n deep-learning python=3.6
source activate deep-learning
</pre>

**Windows**:
<pre>
conda create --name deep-learning python=3.6
activate deep-learning
</pre>
At this point your command line should look something like: (deep-learning) <User>:deep-learning-v2-pytorch <user>$. The (deep-learning) indicates that your environment has been activated, and you can proceed with further package installations.

3.Install PyTorch and torchvision; this should install the latest version of PyTorch.

**Linux** or **Mac**:
<pre>
conda install pytorch torchvision -c pytorch 
</pre>

**Windows**:
<pre>
conda install pytorch -c pytorch
pip install torchvision
</pre>

4.Install a few required pip packages, which are specified in the requirements text file (including OpenCV).

<pre>pip install -r requirements.txt
</pre>

That's it!
Now most of the deep-learning libraries are available to you. Very occasionally, you will see a repository with an addition requirements file, which exists should you want to use TensorFlow and Keras, for example. In this case, you're encouraged to install another library to your existing environment, or create a new environment for a specific project.

Now, assuming your deep-learning environment is still activated, you can navigate to the main repo and start looking at the notebooks:

<pre>
cd
cd deep-learning-v2-pytorch
jupyter notebook
</pre>

To exit the environment when you have completed your work session, simply close the terminal window.
