# Requirements

**Python3 :** is an interpreted high-level programming language for general-purpose programming.

**Jupyter :** lets you create and share interactive code, visualizations, and more. This tool can be used with several programming languages, including Python, Julia, R, Haskell, and Ruby. It is often used for working with data, statistical modeling, and machine learning.

**Numpy :** is a Python library to support large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.

**Pandas :** is a Python library for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

**Scipy :** is a Python library for scientific computing and technical computing. SciPy contains modules for optimization, linear algebra, integration, interpolation, special functions, FFT, signal and image processing, ODE solvers and other tasks common in science and engineering.

**Scikit-learn :** is a free machine learning library in Python. It features various classification, regression and clustering algorithms including support vector machines, random forests, gradient boosting, k-means and DBSCAN, and is designed to interoperate with the Python numerical and scientific libraries NumPy and SciPy.

**MatplotLib :** is a plotting library for the Python programming language and its numerical mathematics extension NumPy. It provides an object-oriented API for embedding plots into applications.

**Seaborn :** is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.

**OpenCV :** is a library of programming functions mainly aimed at real-time computer vision. OpenCV supports the deep learning frameworks TensorFlow, Torch/PyTorch and Caffe.

**PIL :** adds image processing capabilities to your Python interpreter. This library supports many file formats, and provides powerful image processing and graphics capabilities.

# Package Manager Installation

### pip installation

<pre>
    sudo apt update
    sudo apt install python3-pip python3-dev
</pre>

### conda installation

 1. Download the correct version of [Miniconda Installer](https://docs.conda.io/en/latest/miniconda.html) for you.
 2. Install it on your OS following the respective guide [Windows](https://conda.io/projects/conda/en/latest/user-guide/install/windows.html), [Linux](https://conda.io/projects/conda/en/latest/user-guide/install/linux.html), [macOS](https://conda.io/projects/conda/en/latest/user-guide/install/macos.html)

# Setting up a Virtual Environment

Virtual environments are isolated coding environments where you can experiment with various libraries with different versions for your projects without affecting your global package settings. It is extremely helpful in ensuring nothing breaks when you tweak your packages to suite your project requirements. virtualenv and conda both can be used to create python environments, and it's upto you to choose. conda environments are simpler to use when your primary package manager is conda.

### Using conda

You can create a conda environment from YML file (recommended)

<pre>
    conda env create -f environment.yml
</pre>

Or you can create a conda environment for your course project directly with a requirements.txt file. This will install all the packages from your .txt file. (pip package names may differ from conda package names)

<pre>
    conda create -n [NAME OF YOUR ENVIRONMENT] -file [NAME OF YOUR .TXT FILE]
</pre>

OR you can create a empty environment and add packages manually

<pre>
    conda create -n [NAME OF YOUR ENVIRONMENT]
</pre>

Once created, you can activate it using

<pre>
    conda activate [NAME OF YOUR ENVIRONMENT]
</pre>

You can add packages using simply by using

<pre>
    conda install [PACKAGE NAME]
    OR
    pip install [PACKAGE NAME]
</pre>

You can deactivate the environemnt using

<pre>
    conda deactivate
</pre>

You can also view all your enviroments using

<pre>
    conda-env list
</pre>

For more info, please check the conda [documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

### Using virtualenv

<pre>
    sudo pip3 install virtualenv
</pre>

Build new virtualenv

<pre>
    cd $YOUR_PROJECT_DIRECTORY
    virtualenv $NAME 
</pre>

To activate your virtualev

<pre>
    source $NAME/bin/activate
</pre>

# Install the required packages

<pre>
    pip3 install -r requirements.txt
</pre>

or

<pre>
    pip3 install numpy pandas matplotlib scikit-image scikit-learn==0.23.0 jupyter Pillow scipy seaborn xgboost regex catboost imageio imbalanced-learn mlxtend nltk opencv-python
</pre>

# Launching a Jupyter Notebook

<pre>
    jupyter notebook
</pre>
