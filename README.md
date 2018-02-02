# Installing TensorFlow v1.5.0 on Raspberry Pi

This repo contains  pre-built TensorFlow binaries.
 
 If you're looking to run [fully featured TensorFlow](https://github.com/tensorflow/tensorflow) or [Bazel](https://github.com/bazelbuild/bazel) on a Raspberry Pi 3, you're in the right place.


## Installing from Pip
This is the easiest way to get TensorFlow v1.5.0 onto your Raspberry Pi 3. Note that currently, the pre-built binary is targeted for Raspberry Pi 3 running Raspbian 8.0 ("Jessie")

First, install the dependencies for TensorFlow:

```shell
sudo apt-get update

# For Python 2.7
sudo apt-get install python-pip python-dev

# For Python 3.5
sudo apt-get install python3-pip python3-dev
```

Next, download the wheel file from this repository and install it:

```shell
# For Python 2.7
wget https://github.com/asashiho/rpi-tensorflow/releases/download/v1.5.0/tensorflow-1.5.0-cp27-cp27mu-linux_armv7l.whl
sudo pip install tensorflow-1.5.0-cp27-cp27mu-linux_armv7l.whl

# For Python 3.5
wget https://github.com/asashiho/rpi-tensorflow/releases/download/v1.5.0/tensorflow-1.5.0-cp35-cp35m-linux_armv7l.whl
sudo pip3 install tensorflow-1.5.0-cp35-cp35m-linux_armv7l.whl
```

**Note: These are unofficial binaries (though built from the minimally modified official source), and thus there is no expectation of support from the TensorFlow team. Please don't create issues for these files in the official TensorFlow repository.**

