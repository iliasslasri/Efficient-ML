


<img src="images/NAS1.png" width="800">
<img src="images/NAS2.png" width="800">


In ResNet50, bottkeneck block is used to reduce the number of parameters and computation. In this block, 1x1 convolutions are used to reduce the number of channels, then 3x3 convolutions are used to extract features, and finally 1x1 convolutions are used to increase the number of channels. The 3x3 is 9 times more expensive than 1x1 convolutions. REducing the channels before 3x3.

<img src="images/NAS3.png" width="800">

Then ResNeXt introduced grouped convolution, replace the 3x3 convolutions with 3x3 grouped convolutions, with 4 channels each, then concatenate the results and use the 1x1 convolutions. This is more efficient than the bottleneck block in ResNet50.

<img src="images/NAS4.png" width="800">

MobileNet: depthwise-separable block
- Depthwise convolution is an extreme case of group convolution where the group number equals the number of input channels.
- The 1x1 conv is used to mingule the info between the different channels.

<img src="images/NAS5.png" width="800">