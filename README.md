# InfiniTouch: Finger-Aware Interaction on Fully Touch Sensitive Smartphones
This repository contains both the hardware models and specifications for the full-touch smartphone prototype presented in the paper, 
as well as scripts and the model for estimating 3D finger positions on the device as described in the paper. 
Moreover, our dataset can be downloaded in the link provided below.

## Abstract
Smartphones are the most successful mobile devices and offer intuitive interaction through touchscreens. Current devices
treat all fingers equally and only sense touch contacts on the front of the device. In this paper, we present InfiniTouch,
the first system that enables touch input on the whole device surface and identifies the fingers touching the device without
external sensors while keeping the form factor of a standard smartphone. We first developed a prototype with capacitive
sensors on the front, the back and on three sides. We then conducted a study to train a convolutional neural network that
identifies fingers with an accuracy of 95.78% while estimating their position with a mean absolute error of 0.74cm . We
demonstrate the usefulness of multiple use cases made possible with InfiniTouch, including finger-aware gestures and finger
flexion state as an action modifier.

<img src="https://github.com/interactionlab/InfiniTouch/blob/master/teaser_img.png?raw=true" height="300px"> <img src="https://github.com/interactionlab/InfiniTouch/blob/master/Images/Capacitive_Image.png" height="300px">


This work can be cited as follows:
<pre>
@inproceedings{le2018infinitouch,
 author = {Le, Huy Viet and  Mayer, Sven and Henze, Niels},
 title = {InfiniTouch: Finger-Aware Interaction on Fully Touch Sensitive Smartphones},
 booktitle = {Proceedings of the 31th Annual ACM Symposium on User Interface Software and Technology},
 series = {UIST '18},
 year = {2018},
 location = {Berlin, Germany},
 numpages = {13},
 publisher = {ACM},
 address = {New York, NY, USA}
} 
</pre>

## Dataset
The dataset can be downloaded at: (currently uploading). After downloading, place the content of this folder into a folder named 'data'. Place the 'data' folder into the same directory as the Jupyter notebooks. Run the content of these notebooks to create a HDF5 file with which the model can then be trained.

## Prototype
The datasheets of the components that we used in our prototype can be found in the following list of URLs:
- BM10NB(0.8)-40DS-0.4V(51): https://www.datasheets360.com/part/detail/bm10nb-0-8-40ds-0-4v-51/2579290684464631510/
- BM10B(0.8)-40DP-0.4V(51): https://www.datasheets360.com/part/detail/bm10b-0-8-40dp-0-4v-51/-1995328425388918022/
- MPR121QR2: https://www.datasheets360.com/part/detail/mpr121qr2/3714073967749496703/
- MicroUSB Breakout Board: https://cdn-shop.adafruit.com/datasheets/1833_MicroB_20329.pdf
- Tactile Switch: https://cdn-shop.adafruit.com/datasheets/B3F-1000-Omron.pdf
- FH12-50S-0.5SH(05): https://www.datasheets360.com/part/detail/fh12-50s-0-5sh-05/8224149447061018923/
- PCB board + FFC cable: http://diy.shops.hypeltd.com/DIY2//product_info.php?products_id=67
