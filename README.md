# Stable Diffusion XL


## Clone Repo

```sh
sudo apt install dotnet-sdk-7.0 git
git clone https://github.com/Stability-AI/StableSwarmUI
cd StableSwarmUI/
```


## Check your GPU

```sh
lspci | grep -i nvidia
```

## Check your GPU Driver

https://www.nvidia.es/Download/index.aspx?lang=es

## Install Driver for GeForce GT 710 and CUDA Version: 11.4

```sh
sudo apt-get install nvidia-driver-470
```

## Reboot and check drivers 

```sh
reboot
sudo dmesg
nvidia-smi
```

## Check torch latest versions

https://pytorch.org/get-started/locally/

## Check torch previous versions

If there is no version available for that PyTorch version use the previous one available in https://pytorch.org/get-started/previous-versions/ as indicated for CUDA 11.4
https://github.com/pytorch/pytorch/issues/75992

## Install PyTorch for GeForce GT 710 and CUDA Version: 11.4

It is highly recommended to separate the Pytorch installation from the rest of the dependencies to avoid installing the latest versions.

```sh
pip install torch --extra-index-url https://download.pytorch.org/whl/cu113
```

## Execute

```sh
bash launch-linux.sh
```

## Fixes


- The name org.freedesktop.portal.Desktop was not provided by any .service files

```sh
sudo apt install xdg-desktop-portal-gnome
```
