# Installing `zamba`

Zamba has been developed and tested on macOS and Ubuntu Linux for both CPU and
GPU configurations.

## To install `zamba`

### 1. Install prerequisites

Prerequisites:

 - Python 3.7 or 3.8
 - FFmpeg

#### [Python](https://www.python.org/) 3.7 or 3.8

We recommend [Python installation using Anaconda](https://www.anaconda.com/download/) for all platforms. For more information about how to install Anaconda, here are some useful YouTube videos of installation:

 - [Anaconda download link](https://www.anaconda.com/download/)

 - [Windows install video](https://www.youtube.com/watch?v=0OXBHvFeH_U)
 - [macOS installation video](https://www.youtube.com/watch?v=nVlrpNf3EdM)


#### FFmpeg version 4.3

[FFmpeg](https://ffmpeg.org/ffmpeg.html) is an open source library for loading videos of different codecs. Using FFmpeg means that `zamba` can be flexible in terms of the video formats we support. FFmpeg can be installed on all different platforms, but requires some additional configuration depending on the platform. Here are some videos and instructions walking through FFmpeg installation:

 - [FFmpeg download link](https://www.ffmpeg.org/download.html)

 - [Install on Ubuntu or Linux](https://www.tecmint.com/install-ffmpeg-in-linux/).
     - In the command line, enter `sudo apt update` and then `sudo apt install ffmpeg`.
 - [MacOS install video](https://www.youtube.com/watch?v=8nbuqYw2OCw&t=5s)
     - First, install [Homebrew](https://brew.sh/). Then run `brew install ffmpeg`

To check that `FFmpeg` is installed, run `ffmpeg`:

```console
$ ffmpeg

ffmpeg version 4.4 Copyright (c) 2000-2021 the FFmpeg developers
  built with Apple clang version 12.0.0 (clang-1200.0.32.29)
...
```

To check your installed version, run `ffmpeg -version`.

### 2. Install `zamba`

On macOS, run these commands in the terminal (⌘+space, "Terminal"). On Windows, run them in a command prompt, or if you installed Anaconda an anaconda prompt (Start > Anaconda3 > Anaconda Prompt).

To install for development:
```console
$ pip install zamba
```

To check what version of zamba you have installed:
```console
$ pip show zamba
```

To update zamba to the most recent version if needed:
```console
$ pip install -U zamba
```


## Operating Systems that have been tested

### macOS

`zamba` has been tested on macOS High Sierra.

### Linux

`zamba` has been tested on [Ubuntu](https://www.ubuntu.com/) versions 16 and 17.

### Windows

`zamba` has been tested on Windows 10.

## Using GPU

`zamba` is much faster on a machine with a graphics processing unit (GPU), but has also been developed and tested for machines without GPU(s).

To use a GPU, you must be using an
[NVIDIA GPU](https://www.nvidia.com/Download/index.aspx?lang=en-us),
have installed and configured [CUDA](https://developer.nvidia.com/cuda-downloads),
and have installed and configured [CuDNN](https://developer.nvidia.com/cudnn) per
their specifications.