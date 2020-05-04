cd projects

from: https://ngc.nvidia.com/catalog/containers/nvidia:l4t-pytorch
sudo docker pull nvcr.io/nvidia/l4t-pytorch:r32.4.2-pth1.5-py3
sudo docker run -it --rm --runtime nvidia --network host nvcr.io/nvidia/l4t-pytorch:r32.4.2-pth1.5-py3

sudo docker run -it --rm --runtime nvidia --network host -v /home/user/project:/location/in/container nvcr.io/nvidia/l4t-pytorch:r32.4.2-pth1.5-py3
