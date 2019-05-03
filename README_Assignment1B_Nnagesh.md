1. What are Channels and Kernels (according to EVA)?

Kernals- Feature extracters or feature detector or filters or 3x3 matrix: Simple group of weights shared all over the input space.
In other words, kernals can be used with SVM in order to take a new prespective and hopefully allow us translate into for further dimentions in order to find a linear seperate case.

Channels - Collection of kernals (simillar feature of Bags). 
         - image can be divided in to many many different channels
         -number of channels is qual to number of kernals

2. Why should we only (well mostly) use 3x3 Kernels?

 -->There are many reasons and the biggest reason is 3X3 is heavily optimize now. 
 
 -->3x3 is odd number, even numbers we do not have the concept of middle, if it does not have the concept of middle then we can't talk about  things on left and things on right and it is very difficult to create a symmentry using even numbers for e.g if you want to create a triangle with 4X4 with out loosing on the pixels and use all the pixels effectively and you will not able to do that.  if you want to create triangle with 4x4 and you will still using odd number 3x3. 4x4 has 16 numbers and 3x3 has 9 numbers, moving from 3x3 to 4x4 you are adding 7 kernals and we are talking about millians of kernals so literally lot of space is going to be wasted so we need to have odd numbers.
 
 --> if you are using 3X3 it will allows us to reduce number of parameters less to 5x5,7x7,9x9..so on
 
 --> if you are going to use 3X3 kernel in network it will run superfast compare to using other kernal, that is the reason meida, graphic card manufacturers make sure that 3x3 is really really excelarated and using other kernals are very very slow.
 
 
3.How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)








