# shape-detection

**Read my [Medium post](https://towardsdatascience.com/object-detection-with-neural-networks-a4e2c46b4491) on this project**

*Note: Some people reached out and told me that they can't replicate some of the results in this repo. I couldn't find the reason, potentially one of the dependencies changed since I did this project a few years ago. Unfortunately I don't have any notes on which exact setup I used back then. If you find anything, please reach out to me :)*

This is an example of object detection with neural networks (implemented with [keras](https://keras.io/)). The training images contain abstract geometric shapes and can be easily bootstraped. 

The code is split up into several Jupyter notebooks. They increase in complexity:

* Detection of rectangles in numpy arrays: [single-rectangle](single-rectangle.ipynb), [two-rectangles](two-rectangles.ipynb), [multiple-rectangles](multiple-rectangles.ipynb)
* Additional classification between rectangles and triangles: [two-rectangles-or-triangles](two-rectangles-or-triangles.ipynb), [multiple-rectangles-or-triangles](multiple-rectangles-or-triangles.ipynb)
* Application to more complex images (using convnets): [color-multiple-shapes](color-multiple-shapes.ipynb)


![](plots/bw-single-rectangle_prediction.png)


**Requirements**: Python 2.7, keras (v1.0.5), theano or tensorflow, numpy, matplotlib, jupyter, pycairo (only for color-multiple-shapes.ipynb)
