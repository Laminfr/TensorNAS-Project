# TensorNAS-Project

git clone --recurse-submodules https://github.com/alxhoff/TensorNAS-Project.git

# Requirements

`sudo pacman -S cuda cudnn nvidia-dkms nvidia-utils python-tensorflow-opt-cuda`

`python -m pip install -r Demos/DEAP/requirements.txt`

## Linking CUDA libraries

If you get complaints like

`Can't find libdevice directory ${CUDA_DIR}/nvvm/libdevice`

you can either symlink your CUDA libraries, probably in `/opt/cuda` via

`sudo ln -s /opt/cuda/ /usr/local/cuda`

or set `CUDA_DIR` via
