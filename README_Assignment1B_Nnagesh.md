1. What are Channels and Kernels (according to EVA)?

Kernals- Feature extracters or feature detector or filters or 3x3 matrix: Simple group of weights shared all over the input space.
In other words, kernals can be used with SVM in order to take a new prespective and hopefully allow us translate into for further dimentions in order to find a linear seperate case.

Channels -  Collection of kernals (simillar feature of Bags)
number of channels is qual to number of kernals

2. Why should we only (well mostly) use 3x3 Kernels?
In image processing, a kernel, convolution matrix, or mask is a small matrix. It is used for blurring, sharpening, embossing, edge detection, and so on. This is accomplished by doing a convolution between a kernel and an image.

While applying 2D convolutions like 3X3 convolutions on images, a 3X3 convolution filter, in general will always have a third dimension in size. This filter depends on (and is equal to) the number of channels of the input image. So, we apply a 3X3X1 convolution filter on gray-scale images (the number of channels = 1) whereas, we apply a 3X3X3 convolution filter on a colored image (the number of channels = 3).

3.How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)








