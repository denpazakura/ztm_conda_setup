
## Hardware + System

|        |                     |
|--------|---------------------|
| Device | MacBook Pro         |
| Chip   | Apple M3 Pro        |
| System | MacOS Sonoma 14.3.1 |
| Python | 3.12                |

 
## Setup
1. Download [Miniconda](https://docs.anaconda.com/free/miniconda/)
   Miniconda3 macOS Apple M1 64-bit pkg works with M3 as well.
   After a successfull installation you should see (base) once you start a new shell
2. Create a project folder:
   ```
   cd desktop && mkdir project && cd project
   ```
3. In the project folder:
   ```
   project % conda create --prefix ./env pandas numpy matplotlib scikit-learn
   ```
4. If everything's alright, you should see this output:
   
   ```
   Channels:
    - defaults
   Platform: osx-arm64
   Collecting package metadata (repodata.json): done
   Solving environment: done
   ## Package Plan ##
   environment location: /Users/%youruser%/Desktop/project/env
   added / updated specs:
     - matplotlib
     - numpy
     - pandas
     - scikit-learn
   The following packages will be downloaded: ...
   The following NEW packages will be INSTALLED:
   
   Proceed ([y]/n)? 
   ```
   Enter 'y' to proceed.

   ## Working with a conda environment
   
6. After everything's been downloaded, you'll get a hint from conda:
   ```
   # To activate this environment, use                                             
   #                                                                               
   #     $ conda activate "/Users/%youruser%/Desktop/project/env"                                                                         
   #                                                                               
   # To deactivate an active environment, use                                      
   #                                                                               
   #     $ conda deactivate  
   ```
   
  7. Activate the environment:
     
      ```
      conda activate /Users/%youruser%/Desktop/project/env
      ```  

  9. Install JupyterLab:
     
      ```
      conda install -c conda-forge jupyterlab 
      ```
  10. Get info about current environment:

      ```
      conda info
      ```
  11. Start Jupyter notebook:
      ```
      jupyter lab
      ```    
