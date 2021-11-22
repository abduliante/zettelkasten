# Commands I might use later

### * Conda enviroment not launching in jupyter notebook?
Probably ipykernel not installed in your enviroment, install ipykernel
``` conda install -c anaconda ipykernel ```
Next, in your enviroment, link your ipykernel to your enviroment
``` python -m ipykernel install --user --name=[NAME_OF_YOUR_ENVIROMENT] ```
