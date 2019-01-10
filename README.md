These notebooks  aim at teaching you the fundamentals of Python3 and the following libraries:
 Numpy, matplotlib, pandas.

 # Installation

 First, you will need to install [git](https://git-scm.com/), if you don't have it already.

 Next, clone this repository by opening a terminal and typing the following commands:

     $ cd development/  # or whatever your  development directory is
     $ git clone https://github.com/sachin80/nps_tutorials.git
     $ cd nps_tutorials

 If you do not want to install git, you can instead download [master.zip](https://github.com/sachin80/nps_tutorial/archive/   master.zip), unzip it, rename the resulting directory to `nps_tutorials` and move it to your development directory.

 ## Using Anaconda
 When using Anaconda, you can optionally create an isolated Python environment dedicated to this project. This is             recommended as it makes it possible to have a different environment for each project (e.g. one for this project), with       potentially different libraries and library versions:

     $ conda create -n mltutorials python=3.5 anaconda
     $ conda activate mltutorials

 This creates a fresh Python 3.5 environment called `mltutorials` (you can change the name if you want to), and it activates  it. This environment contains all the scientific libraries that come with Anaconda. This includes all the libraries we will  need (NumPy, Matplotlib, Pandas, Jupyter and a few others), except for TensorFlow, so let's install it:

     $ conda install -n mltutorials -c conda-forge tensorflow

This installs the latest version of TensorFlow available for Anaconda (which is usually *not* the latest TensorFlow         version) in the `mltutorials` environment (fetching it from the `conda-forge` repository). If you chose not to create an   mltutorials` environment, then just remove the `-n mltutorials` option.

 Next, you can optionally install Jupyter extensions. These are useful to have nice tables of contents in the notebooks, but  they are not required.

     $ conda install -n mltutorials -c conda-forge jupyter_contrib_nbextensions

 ## Starting Jupyter
 If you want to use the Jupyter extensions (optional, they are mainly useful to have nice tables of contents), you first    need to install them:

     $ jupyter contrib nbextension install --user

 Okay! You can now start Jupyter, simply type:

     $ jupyter notebook

 This should open up your browser, and you should see Jupyter's tree view, with the contents of the current directory. If   your browser does not open automatically, visit [localhost:8888](http://localhost:8888/tree). Click on `index.ipynb` to get  started!

