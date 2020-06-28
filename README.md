# Tools for Reproducible Science
- 
- Version Control Systems (Git and Github)
- Computational Notebooks (Jupyter)
- Public Interactive Notebooks
Allows researchers to quickly create and share computational environments needed to interact with research code and data.
Tool : Binder 
  
In particular, how to share notebooks and allowing running them or modify  them interactively.  
  
  Idea: Binder pulls code from repository(GitHub). Packages needed and detailed in requirements.txt are installed in the environment in the cloud.  
  
  How to share our static jupyter notebook with Binder:  
  
  1. Create a repository containing a requirements.txt fiel (packages are detailed woth versions)
  spaces "=="
  ```
  matplotlib==3.2.1
  ```
  2. Upload the static versions of the notebooks to the repository
  3. Create the computational environment in Binder (we use a github repository). Copying the url from our repository.
  
- Repositories (Zenodo) launched on May 2013
