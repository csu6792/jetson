# jetson

# yolov5
```
sudo apt-get update

wget https://nvidia.box.com/shared/static/9eptse6jyly1ggt9axbja2yrmj6pbarc.whl -O torch-1.6.0-cp36-cp36m-linux_aarch64.whl

sudo apt-get install python3-pip libopenblas-base libopenmpi-dev 

pip3 install Cython

pip3 install numpy torch-1.6.0-cp36-cp36m-linux_aarch64.whl

pip3 install Pillow

pip3 install matplotlib

pip3 install tqdm
```

```
sudo apt-get install libjpeg-dev zlib1g-dev libpython3-dev libavcodec-dev libavformat-dev libswscale-dev

git clone --branch v0.7.0 https://github.com/pytorch/vision torchvision

cd torchvision

export BUILD_VERSION=0.7.0

sudo python3 setup.py install
```

# tensorflow

**check jetpack**
```
head -n 1 /etc/nv_tegra_release
```

**for 4.3**
```
sudo apt-get install libhdf5-serial-dev hdf5-tools libhdf5-dev zlib1g-dev zip libjpeg8-dev
sudo apt-get install python3-pip
sudo pip3 install -U pip
sudo pip3 install -U numpy grpcio absl-py py-cpuinfo psutil portpicker six mock requests gast h5py astor termcolor protobuf keras-applications keras-preprocessing wrapt google-pasta
# TF-2.x
sudo pip3 install --pre --extra-index-url https://developer.download.nvidia.com/compute/redist/jp/v43 tensorflow==2.1.0+nv20.3
# TF-1.15
sudo pip3 install --pre --extra-index-url https://developer.download.nvidia.com/compute/redist/jp/v43 tensorflow==1.15.2+nv20.3
```
