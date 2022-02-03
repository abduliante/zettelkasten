# Commands I might use later

### * Conda enviroment not launching in jupyter notebook?
Probably ipykernel not installed in your enviroment, install ipykernel
``` conda install -c anaconda ipykernel ```
Next, in your enviroment, link your ipykernel to your enviroment
``` python -m ipykernel install --user --name=[NAME_OF_YOUR_ENVIROMENT] ```

### * Jupyter not opening directly to browser on WSL?
First you have to set the ```startingDirectory``` to WSL. This can be edited in Windows Terminal. Now for Jupyter to work on WSL; first generate notebook config using ```jupyter notebook --generate-config``` then open your favorite editor on ```~/.jupyter/jupyter_notebook_config.py```. Uncommit and change ```c.NotebookApp.use_redirect_file``` to be ```False```. Next, fire up your ```~/.bashrc``` and add your favorite browser path ```export BROWSER='/mnt/YOUR/BROWSER/PATH/chrome.exe'```. Dont forget to ```source ~/.bashrc``` for immediate results.