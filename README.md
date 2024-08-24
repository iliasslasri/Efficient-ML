
# Efficient ML

This repository also contains my learning on advanced efficient ML.


# Papers to read
[Deep compression ](https://arxiv.org/pdf/1510.00149)

[EIE: Efficient Inference Engine on Compressed Deep Neural Network](https://arxiv.org/pdf/1602.01528)
[Learning both Weights and Connections for Efficient Neural Networks](https://arxiv.org/pdf/1506.02626)

# Papers I'm reading

[A White Paper on Neural Network Quantization](https://arxiv.org/pdf/2106.08295)


### Programming advice for me :
- Use sanity checks :
 Python : ``` assert isinstance(prune_ratio, (float, list)) ```, C++ : ``` static_assert(std::is_floating_point<T>::value, "T must be floating point"); ```, take a look at ``` def channel_prune(model: nn.Module,prune_ratio: Union[List, float]) -> nn.Module ``` in lab1.ipynb
- deepcopy ;)