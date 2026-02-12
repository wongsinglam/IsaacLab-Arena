## Clone everything
- git clone git@github.com:isaac-sim/IsaacLab-Arena.git
- git submodule update --init --recursive

## Install pre-requirements
- pip install -r pre_requirements.txt

## Install isaac-sim 
- pip install "isaacsim[all,extscache]==5.1.0" --extra-index-url https://pypi.nvidia.com
- pip install -U torch==2.7.0 torchvision==0.22.0 --index-url https://download.pytorch.org/whl/cu128

## Install IsaacLab
- cd submodules/IsaacLab
- ./isaaclab.sh -i

## Install IsaacLab-Arena
- cd ../../
- pip install -e .