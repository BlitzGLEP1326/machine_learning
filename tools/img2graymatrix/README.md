This directory contains a Python script `img2graymatrix.py` which converts an image to grayscale and outputs the pixel values as a matrix to stdout which can be loaded in Octave vie the `load` command. The output value for each pixel is in the range [0,255].

If the image has width `w` and height `h` the output is a `h x w` matrix.

Example usage:

```./img2graymatrix.py cat.png > cat.txt```

In Octave the image can be loaded and displayed with the following commands:

```load('cat.txt'), colormap(gray), imagesc(cat);```
