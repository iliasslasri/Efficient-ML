- Lecture slides : [dropbox](https://www.dropbox.com/scl/fi/lfcbzfbr3t2z9joz9ymt0/lec07.pdf?rlkey=yzx2o9bjnhzi5tstwevmcu6qv&e=2&dl=0)


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


In NAS, the search space is the space of all possible neural network architectures. The search space is huge, so we need to use a search strategy to find the best architecture. The search strategy can be random search, grid search, evolutionary search, reinforcement learning, etc.

Search strategies:
  - Grid search
  - Random search
  - Reinforcement learning
  - Gradient descent
  - Evolutionary search

**Grid search**

<img src="images/NAS6.png" width="800">
<img src="images/NAS7.png" width="800">


**Random search**
Random search is the simplest search strategy, but it is not efficient. It is like a blind search, instead of using the information from the previous searches, just randomly search the space.

**Reinforcement learning**

<img src="images/NAS8.png" width="800">