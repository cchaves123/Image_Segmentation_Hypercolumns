# Image_Segmentation_Hypercolumns

See report.pdf for an in-depth explanation of my project.

Image segmentation is essentially pixel-classification. That is, given an image, we want to build a model to predict which class every pixel in the image belongs to. This project does this using hypercolumns.

What is a hypercolumn? When an image is passed into a CNN, it creates activation tensors at each layer in the net. Suppose all of these activations were then upsampled/cropped to the size of the original image. The idea behind hypercolumns is that the activation value at a given location in a layer contains information about the corresponding pixel in the image. So, we can aggregate activation values by location into feature vectors, and then use these vectors for pixel classification.
