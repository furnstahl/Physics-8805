
### Installation of Physics-8805 Jupyter notebooks from GitHub by command line

Go to the location where you want the notebook files.

Download the 8805 repository from GitHub and enter the directory `Physics-8805` which should have been created on your computer:

    git clone https://github.com/furnstahl/Physics-8805.git
    cd Physics-8805

The notebooks that we will be using depend on several scientific python modules (see the list in environment.yml) and require a python3.x installation based on Anaconda. 

These python modules and their dependencies are best installed using ``conda`` by creating
a virtual environment:

	conda env create

which reads the `environment.yml` file in your current directory (in this case the one in Physics-8805).  This will take a while; be patient!  You will see a listing being generated like:
        
       Downloading and Extracting Packages
       scikit-learn-0.21.3  | 5.9 MB    | ##################################### | 100% 
       glib-2.58.3          | 3.1 MB    | ##################################### | 100% 
       libcxx-8.0.1         | 1000 KB   | ##################################### | 100% 
       scipy-1.3.1          | 18.1 MB   | ##################################### | 100% 
etc. (it will be a pretty long list and not necessarily be in this order).  Then you'll see

       Preparing transaction: done
       Verifying transaction: done
       Executing transaction: done 
where "done" appears when it has finished.  If all is well at the end, you'll get a success message.  If it fails, email the message you get to furnstahl.1@osu.edu.

Some packages might not be found in the default conda channels. One
can either specify relevant package channel(s) in the environment.yml
file (as done here), or add them to the default conda channel configuration via, e.g,

	conda config --append channels conda-forge

You shouldn't need to do this for the initial setup.

Once the virtual environment has been created it can be activated (the name "8805-env" was specified in the environment.yml file):

    conda activate 8805-env

To deactivate the virtual environment:

    conda deactivate

Note that earlier versions of conda used 'source' instead of 'conda'
to activate environments. If you have an earlier version of conda you
might have to do

    conda update conda

Note that there are also other options ('venv', 'pipenv') for creating virtual
environments that includes the python version and packages that we will be using.

Once the environment is set up and activated, you are encouraged to run the test Jupyter notebook:

    cd intro
    jupyter notebook Anaconda_Bayes_test.ipynb

Other notebooks can be found in the subdirectories under topics.

### Updating your conda environment for 8805

Go to the `Physics-8805` directory you created by cloning the class repository.  This is where the relevant `environment.yml` file is stored.  This file defines the environment and will be occasionally updated to add additional modules.  
You can update to the new environment with:

    conda deactivate
    conda env update 
    
Now if you activate the environment again:

    conda activate 8805-env

you will have access to the new packages.
