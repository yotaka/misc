
# Local setup and misc links

[jupyter workbooks](http://localhost:8888/tree/Documents/IPython)

[Tensorboard](http://veda:6006/#graphs&run=.)

[models on GitHub](https://github.com/tensorflow/models)

## Launch

Tensorboard:
```
tensorboard.exe --logdir=./tryout.tf/
```

Jupyter:
```
jupyter-notebook --no-browser
```


# Installation

Installed 
* Python (current version), 
* NVidia CUDA SDK (older version since the newest version does not work with Tensorflow), 
* NVidias DNN DLL, 
* Visual Studio Community Edition (C++, Python, Windows 10 SDK, older Build Pipeline, to build and run NVidia examples and utilities which are not shipped binary anymore),
* Tensorflow, 
* IPython, 
* Jupyter

# Post-installation verification

see files in directory:
* `hello_world.log`
* `deviceQuery_bandwithTest.log`

# First tutorial: Mandelbrot

I chose this one as it does not actually include DNNs and I thought it might be a good introduction to Tensorflow basics.

[Link](https://www.tensorflow.org/tutorials/mandelbrot)

It's quite good to check if everything is set up correctly, T


# Second tutorial: MNIST

[Link](https://www.tensorflow.org/tutorials/layers)

