# Image-Style-Transform
In our project, we use the perceptual loss functions for training feed-forward networks instead of the traditional per-pixel loss between the output and ground-truth images (style image and content image) for image style transformation. The method we use can do the transformation almost in real- time via GPU. We divide our neural network into two parts, the image transform net and the loss net. For the image transform net we compare the result of two image transform net, with or without residual blocks. By the method of extracting high-level features from pre-trained loss net, we can optimize the quality of images generated. Our loss function contains three different parts, that is, style reconstruction loss, feature reconstruction loss and total variation loss for style penalty, content penalty and spatial smoothness in the output image separately. Also, we do a multiple style transfer and make some improvements for the quality of the transformed image.