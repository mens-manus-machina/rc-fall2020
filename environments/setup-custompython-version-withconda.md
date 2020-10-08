# Q: How can I create a custom Python environment for a particular project?  https://joss.theoj.org/papers/10.21105/joss.01356

# A: Conda/minicoda is one way to do this.

# Installing conda via command line


1. create a custom directory to work and switch to working in that directory
  ```
  mkdir myspecialenv
  cd    myspecialenv
  ```


2. download conda install script and install the conda software in a sub-directory called
  ```
  curl https://repo.anaconda.com/archive/Anaconda3-2020.07-MacOSX-x86_64.sh > Anaconda3-2020.07-MacOSX-x86_64.sh
  chmod +x Anaconda3-2020.07-MacOSX-x86_64.sh
  ./Anaconda3-2020.07-MacOSX-x86_64.sh -p conda3
  ```
  
3. activate the base conda environment and check python version (it will be a very recent version)
  ```
  source conda3/bin/activate
  python -V
  ``` 

4. now create a new conda environment based on python 3.7 (or another version) and activate
  ```
  conda create -n py37 python=3.7
  conda activate py37
  ```
  
5. now check the version and it should be python 3.7
  ```
  python -V
  ```
  
6. to deactivate the conda environments use
  ```
  conda deactivate
  conda deactivate
  ```
  
7. to reactivate the environment 
  ```
  cd    myspecialenv
  source conda3/bin/activate  
  conda activate py37
  ```
  
Conda can be used in this way to create multiple different evironments. 
