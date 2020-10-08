# Q. What is a way to install serotools? ( https://joss.theoj.org/papers/10.21105/joss.02556 ). 

Serotools appears to be command ine program that invokes Python, but is not run from within a Python shell. See for example https://serotools.readthedocs.io/en/latest/usage.html#usage

1. install Python via conda.

   ```
     curl https://repo.anaconda.com/archive/Anaconda3-2020.07-MacOSX-x86_64.sh > Anaconda3-2020.07-MacOSX-x86_64.sh
chmod +x Anaconda3-2020.07-MacOSX-x86_64.sh
./Anaconda3-2020.07-MacOSX-x86_64.sh -p conda3
   ```
2. 

  ```
  source conda3/bin/activate
  python -V
  ```
  
 3. 
 
  ```
   conda create -n serotools python=3.8
   conda activate serotools 
  ```
  
 4. 
  ```
    pip install --user serotools
  ```
  
 5.
  ```
   ~/.local/bin/serotools query -s 'Paratyphi A'
  ```
