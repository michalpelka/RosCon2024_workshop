---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
![](assets/100-2.gif)

Welcome to the Hand-Held Mobile Mapping System for Large-Scale Surveys workshop.
During the workshop attendees are expected to perform mapping tasks with handheld devices and 
process results.
The device is an open hardware project available here: [mandeye](https://github.com/JanuszBedkowski/mandeye_controller).

You can assemble your device, but we will bring a dozen devices for you.

## Notes 💡
> **_NOTE1:_** Please revisit this page before the workshop to get the latest updates

> **_NOTE2:_** All refered gitthub projects [mandeye](https://github.com/JanuszBedkowski/mandeye_controller), 
 [HDMapping](https://github.com/MapsHD/HDMapping) are open to you contributions

## Prerequesities

The [project HDMapping](https://github.com/MapsHD/HDMapping) is supported for Windows and Linux.
We recommend the following distributions:
- Windows 11
- Windows 10
- Ubuntu 22.04
- Ubuntu 24.04

The machine you are running should have plenty of RAM. 
For small-scale experiments, 16 GB should be enough. 
Consider adjusting virtual memory to utilize disk space, details can be found [here](https://github.com/MapsHD/HDMapping/blob/main/doc/virtual_memory.md)

## Software
The project is available with binaries both for Windows and Linux.

### Ubuntu, prebuilt packages

The prebuilt package is done automatically and can be found here for version [0.58.0](assets/hd_mapping-0.58.0-Linux.deb)

```
sudo apt-get install freeglut3-dev libeigen3-dev liblaszip-dev
sudo dpkg -i hd_mapping-0.58.0-Linux.deb 
```

### Windows, prebuilt packages

Visit [release](https://github.com/MapsHD/HDMapping/releases/tag/v0.58) page and download binaries.

### Build from source

The HDMapping project, can be built from source. It comes with all necessary 3rd party libraries.

```
git clone https://github.com/MapsHD/HDMapping.git
cd HDMapping
mkdir build
git submodule init
git submodule update --recursive
cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make -j
```


## Sample Dataset to download

We will work with the data you capture, however please download following datasets - as more advanced usecase.

### Underground parking
Ground truth:\
![](assets/undeground_groundtruth.png)
Dataset:
![]()
Download link:\
[link](https://drive.google.com/file/d/1W0ep2TYIF-pnI9gBNBv2fd7fcVuMyCmI/view?usp=sharing)

### Roccastrada
[link](https://drive.google.com/file/d/1OinqqI4D9E6hQL1Kk073yuV2fqtgUkKf/view?usp=sharing)

### Forest 
[link](https://drive.google.com/file/d/1uKrv7YPvdlkTGh4oeNxvAKVvNXaovBPL/view?usp=sharing)

### Rubble Field
[link](https://drive.google.com/file/d/1FtQYMnmfFqVPvUdJXn54eb_gp-M_TMn7/view?usp=sharing)

### Cave
[link](https://drive.google.com/file/d/1DdgTccNPSKctF08O97XoNRK9XZ54QXst/view?usp=sharing)

## 3rd party SLAM evaluation with HDMapping

TBD
