TWRP Device Tree for OPPO A12/A11k
===========================================

OPPO A12/A11k is a budget range smartphone from OPPO, announced in April 2020.

## Status

**Working**:


**Not working**:

1. Decryption


## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
OS	| Android 9.0 (pie)	
CPU     | Octa-core (4x2.35 GHz Cortex-A53 & 4x1.8 GHz Cortex-A53)
Chipset | Mediatek MT6765 Helio P35 (12 nm)
GPU     | PowerVR GE8320
Memory  | 3GB/4GB RAM
Storage | 32GB/64GB
MicroSD | up to 64 GB
Battery | Non-removable Li-Ion 4230 mAh battery
Resolution | 720 x 1520 pixels, 19:9 ratio (~270 ppi density)
Camera (Rear)  | 13 MP, f/2.2, (wide), 1/3.1", 1.12µm, PDAF & 2 MP, f/2.4, (depth)
Rear Camera Features | LED flash, HDR, panorama
Video	| 1080p@30fps	
Camera (Front)  | 5 MP, f/2.0, 1/5", 1.12µm
Features| Fingerprint (rear-mounted), accelerometer, gyro, proximity, compass	

## Device picture

![OPPO A12](https://fdn2.gsmarena.com/vv/pics/oppo/oppo-a12-1.jpg "OPPO A12")



## Getting Started ##
---------------

To get started with OMNI sources to build TWRP, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

# repo init

To initialize your local repository using the OMNIROM trees to build TWRP, use a command like this:

    repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

To initialize a shallow clone, which will save even more space, use a command like this:

    repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

# repo sync

 Then to sync up:

    repo sync 

## To Build ##
---------------

Build the TWRP recovery using below command.

    cd <source-dir>; export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch omni_OP4BFB-eng; mka recoveryimage

## NOTE

Most of the work here is from internet. Thanks to https://github.com/buddi56.
