# QUVCView 

A Qt application for controlling and viewing video from UVC compatible USB camera devices. It is made using Qt (GUI), libuvc (camera communication), and OpenCV (video writing). This app provides zoom-in/out that GUVCView doesn't have. I updated the original app from https://github.com/erikmwerner/QUVCView to the recent Qt6 and use pkg-config to manage the compliation on linux.

![QUVC View](QUVCView_screenshot.jpg "QUVC View")

## Features
* UVC device discovery
* Read/write most standard UVC device controls (exposure, focus, brightness, contrast, etc..)
* Save videos
* Save still images
* Automatically save sequences of images
* Pinch-to-zoom gesture support

## Dependencies
* Qt6
* apt install libopencv-dev
* apt install libuvc-dev

> **NOTE:** You may run `pkg-config --libs libuvc` and `pkg-config --libs opencv4` for checking the other missing dependencies 

## Thanks
Many of the UVC controls were modified from [UVC Camera Control for Mac OS X](https://phoboslab.org/log/2009/07/uvc-camera-control-for-mac-os-x)

## See also
* [openCV](https://opencv.org)
* [libusb](https://libusb.info)
* [libuvc](https://github.com/libuvc/libuvc)
* [VVUVCKit](https://github.com/mrRay/VVUVCKit)
* [UVC Camera Control for Mac OS X](https://phoboslab.org/log/2009/07/uvc-camera-control-for-mac-os-x)
