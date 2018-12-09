Copyright (c) 2018, The TurtleCoin Developers
Copyright (c) 2018, The Nibble Developers
Please see the included LICENSE file for more information.

### Installing

### How To Compile

#### Linux

##### Prerequisites

- You will need the following packages: boost (1.55 or higher), rocksdb, cmake, git, gcc (4.9 or higher), g++ (4.9 or higher), make, GNU readline, and python. Most of these should already be installed on your system.
- For example on Ubuntu: `sudo apt-get install -y build-essential python-dev gcc g++ git cmake libboost-all-dev libreadline-dev`

##### Building

- `git clone -b master https://https://github.com/Sudosups/NBX.git`
- `cd plenteum`
- `mkdir build && cd $_`
- `cmake -DCMAKE_BUILD_TYPE=Release -DSTATIC=true ..`
- `make`

#### Windows

##### Prerequisites

- Install [Visual Studio 2017 Community Edition](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15&page=inlineinstall)
- When installing Visual Studio, it is **required** that you install **Desktop development with C++**
- Install the latest version of [Boost](https://sourceforge.net/projects/boost/files/boost-binaries/1.68.0/boost_1_68_0-msvc-14.1-64.exe/download) - Currently Boost 1.68.

##### Building

- From the start menu, open 'x64 Native Tools Command Prompt for vs2017'.
- `cd <your_lumeneo_directory>`
- `mkdir build`
- `cd build`
- `set PATH="C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\IDE\CommonExtensions\Microsoft\CMake\CMake\bin";%PATH%`
- `cmake -G "Visual Studio 15 2017 Win64" .. -DBOOST_ROOT=C:/local/boost_1_68_0` (Or your boost installed dir.)
- `MSBuild TurtleCoin.sln /p:Configuration=Release /m`

The binaries will be in the `src/Release` folder when you are complete.
