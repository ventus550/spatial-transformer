# SpatialTransformer

Spatial Transformer Networks (STN) is a type of neural network module that can be inserted into a convolutional neural network (CNN) to enable the network to spatially transform input images in order to enhance the geometric invariance of the network. STNs allow the network to learn how to spatially transform the input images in order to better handle variations such as rotations, scaling, and translations.

![image](https://user-images.githubusercontent.com/58316065/236997990-51b23630-48cb-43af-b917-851291b10923.png)


An STN consists of three main components:

- Localization Network: This is a small CNN that learns to predict the parameters of the transformation that needs to be applied to the input image. The output of this network is a set of transformation parameters that can be used to perform the spatial transformation.

- Grid Generator: This component takes the transformation parameters predicted by the localization network and generates a grid of coordinates that define the transformation.

- Sampler: This component samples the input image using the grid generated by the grid generator to produce the transformed output.

![image](https://github.com/ventus550/SpatialTransformer/blob/main/spatial_transformer_demo.gif)

By incorporating an STN module into a CNN, the network is able to learn how to transform the input images in a way that enhances the network's ability to recognize objects that have undergone different types of spatial transformations.
