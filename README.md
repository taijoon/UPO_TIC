# UPO_TIC(Thermal Imaging Camera)

## Device
 - 아이리스솔루션
 - link : http://www.irsolution.co.kr/ 

## install package
 - [list link](./list_package.md)

## cmake setting
 - [cmake](./cmake_setting.md)

## install opencv4
<pre>
wget -O opencv.zip https://github.com/opencv/opencv/archive/4.2.0.zip
wget -O opencv_contrib.zip https://github.com/opencv/opencv_contrib/archive/4.2.0.zip
unzip opencv.zip
unzip opencv_contrib.zip
</pre>

## copy lib env
 - gcc-linaro-6.3.1-2017.05-i686_arm-linux-gnueabihf-g++ 폴더 라이브러리 사용

## execution
<pre>
g++ main.cpp Usb.cpp -L. -lthermometry -lSimple -lm -lpthread -lpot -lusb-1.0 -o main1 `pkg-config opencv4 --libs --cflags`
export LD_LIBRARY_PATH=./
./main1
a
</pre>
