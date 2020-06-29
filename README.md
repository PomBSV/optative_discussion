# Tools for Reproducible Science
Guillaume Witz (ScITS)

- This course aims to show the ways to reproduce research.
- Version Control Systems (Git and Github)
- Computational Notebooks (Jupyter)
- Public Interactive Notebooks
Allows researchers to quickly create and share computational environments needed to interact with research code and data.
Tool : **Binder** 
Software project to share interactive, reproducible environments.
The project maintains core libraries and documentation for running Binder services, which make those projects available, 
as well as **BinderHub**, a tool for deploying such services via common cloud computing environments. A public BinderHub 
portal is hosted by the community at mybinder.org

***Binder from the users point of view:***
Binder pulls code from repository(GitHub). Packages needed and detailed in requirements.txt are installed in the environment in the cloud. My notebook instead of a static image as in the case of a pdf could be shown.

***Binder internals:***

![](images/image1.png?raw=true)

One of the basis projects within Binder, is the so called **repo2docker** project.
It takes a repository and turns it into a Docker image. (Why Docker : to automate steps that human would do to publish a repository and interact with it) . 
    Problem: users often have compute environments with different package or software versions. 
             Sometimes an specific version software/package is needed.
And a Docker image is a file is the solution, comprised of multiple layers, that is used to execute code in a Docker container.






In particular, how to share notebooks and allowing running them or modify  them interactively.  
  
  
  How to share our static jupyter notebook with Binder:  
  
  1. Create a repository containing a requirements.txt fiel (packages are detailed woth versions)
  spaces "=="
  ```
  matplotlib==3.2.1
  ```
  2. Upload the static versions of the notebooks to the repository
  3. Create the computational environment in Binder (we use a github repository). Copying the url from our repository.
  
- Repositories (Zenodo) launched on May 2013
