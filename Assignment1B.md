## Channels and Kernels/Filters

Channels are input image features if image has 3 features then we will have 3 channels. The number of output filters is equivalent to the number of input channels 

The Kernel/Filters will be able to detect edges, adjacent, texture, patterns, partial objects and objects over input image. The convolution kernel/filter is a small matrix that will have numbers in each cell.

The kernel/filters slide over an image and multiple everything element by element wise and sum of all will be the output.

Every image can be considered as a matrix of pixel values. If we apply 3X3 filter on 6X6 image output will be 4X4.

Number of kernels in each layer can change significantly. The more complex the dataset you expect networks with more kernels perform better.

Deep leaning network will learn the kernel/filters values through the backpropagation


## Why 3X3?
3x3 kernel is heavily optimized

3x3 is odd number, cartelizing pixels of an image is possible with odd numbers where as cartelizing pixels of an image is not possible with even numbers (4x4)

3x3 kernel is faster than other kernels

Number of parameters are less than other kernels

if we do convolution on 5x5 image with 5x5 kernel the out put is 1X1

if we do convolution on 5x5 image with 3x3 kernel the out put is 3X3 and if we do 3x3 convolution again we get the 1x1 

5x5 =25 params, 3x3 + 3x3 = 9+9 =18 params


## How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)
we neeed to perform 99 3x3 convolution operations to reach 1x1 
199x199(3x3)|197x197(3x3)|195x195(3x3)|193x193(3x3)|191x191(3x3)|189x189(3x3)|187x187(3x3)|185x185(3x3)|183x183(3x3)|181x181(3x3)|179x179(3x3)|177x177(3x3)|175x175(3x3)|173x173(3x3)|171x171(3x3)|169X169(3x3)|167x167(3x3)|165x165(3x3)|163x163(3x3)|161x161(3x3)|159x159(3x3)|157x157(3x3)|155X155(3x3)|153x153(3x3)|151x151(3x3)|149x149(3x3)|147x147(3x3)|145x145(3x3)|143X143(3x3)|141x141(3x3)|139x139(3x3)|137x137(3x3)|135x135(3x3)|133x133(3x3)|131x131(3x3)|129x129(3x3)|127x127(3x3)|125x125(3x3)|123x123(3x3)|121X121(3x3)|119x119(3x3)|117x117(3x3)|115x115(3x3)|113x113(3x3)|111x111(3x3)|109x109(3x3)|107X107(3x3)|105x105(3x3)|103X103(3x3)|101x101(3x3)|99x99(3x3)|97x97(3x3)|95x95(3x3)|93x93(3x3)|91x91(3x3)|89x89(3x3)|87x87(3x3)|85x85(3x3)|83x83(3x3)|81x81(3x3)|79x79(3x3)|77x77(3x3)|75x75(3x3)|73x73(3x3)|71x71(3x3)|69X69(3x3)|67x67(3x3)|65x65(3x3)|63x63(3x3)|61x61(3x3)|59x59(3x3)|57x57(3x3)|55X55(3x3)|53x53(3x3)|51x51(3x3)|49x49(3x3)|47x47(3x3)|45x45(3x3)|43X43(3x3)|41x41(3x3)|39x39(3x3)|37x37(3x3)|35x35(3x3)|33x33(3x3)|31x31(3x3)|29x29(3x3)|27x27(3x3)|25x25(3x3)|23x23(3x3)|21X21(3x3)|19x19(3x3)|17x17(3x3)|15x15(3x3)|13x13(3x3)|11x11(3x3)|9x9(3x3)|7X7(3x3)|5x5(3x3)|3X3(3x3)|1x1|
