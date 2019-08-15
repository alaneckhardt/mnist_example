# MNIST with BagNet

A very simple impelentation of the idea in this paper:
https://openreview.net/pdf?id=SkfMWhAqYQ
applied to MNIST, which isn't really the point of the paper, as there is no texture in MNIST. But I was curious how this approach will perform here.

The idea is to divide the picture into small patches, each patch is processed separately and votes on its class. 
Then the mean of the votes is taken as the class of the whole image.
The point is that it performs well on Imagenet etc., where the texture is sufficient to guess the class.

To run the notebook, please install pytorch, torchvision and matplotlib.

Installation using conda:
```
conda install jupyter matplotlib pytorch torchvision cudatoolkit=10.0 -c pytorch
```
or other installation methods here: https://pytorch.org/get-started/locally/
