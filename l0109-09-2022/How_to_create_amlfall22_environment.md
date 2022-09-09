## Downloading and installing Python using Anaconda
`https://www.anaconda.com/products/distribution`

## Creating a vitual python environment for AML Fall 2022
### Installing the most recent python engine and the spyder IDE
`conda create -n amlfall22 python spyder`

`conda activate amlfall22`

`conda install -c conda-forge pyqtwebengine`

### If GPU is available for tensorflow
`conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0`

### tensorflow for CPU and GPU
`pip install tensorflow`

### Jupyter notebook will be usefull
`conda install -c anaconda jupyter`

### Other libraries we will be using throughout the course
`conda install numpy pandas scikit-learn matplotlib`

### Verifying Tensorflow GPU installation:
`python -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"`
> [PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')]


### Alternative install using amlfall22.yml
`conda env create -f amlfall22.yml`