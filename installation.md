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

# Install additional dependencies
pip install onnxruntime==1.23.2 lightwheel-sdk==1.0.1 vuer[all]==0.0.70 qpsolvers==4.8.1
pip install numpy==1.26.0 # Isaac Sim 5.1 depends on numpy==1.26.0, this will be fixed in next release