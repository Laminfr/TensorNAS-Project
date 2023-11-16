# TensorNAS-Project

git clone --recurse-submodules https://github.com/Laminfr/TensorNAS-Project.git

# Requirements

`sudo pacman -S cuda cudnn nvidia-dkms nvidia-utils python-tensorflow-opt-cuda`

`python -m pip install -r Demos/DEAP/requirements.txt`

## Linking CUDA libraries

If you get complaints like

`Can't find libdevice directory ${CUDA_DIR}/nvvm/libdevice`

you can either symlink your CUDA libraries, probably in `/opt/cuda` via

`sudo ln -s /opt/cuda/ /usr/local/cuda`

or set `CUDA_DIR` and some other dependencies by exporting them to your `.bashrc` or your `.profile`.

Example, adding the following to your `.bashrc`

```
export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:/opt/cuda/lib64"
export CUDA_HOME=/opt/cuda/
export PATH="/opt/cuda/bin:$PATH"
export CPATH="/opt/cuda/include:$CPATH"  
```
