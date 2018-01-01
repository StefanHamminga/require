# require

Very simple C++ library to specify a required language standard or feature in a header or source.

Some language features of newer standards have clear errors indicating use of an outdated standard. Because this is not always the case these helper includes will enforce a strong and clear error instead. Especially when combined with `-Wfatal-errors`.

## Installation

```bash
git clone https://github.com/StefanHamminga/require.git
cd require
mkdir build

# Prepare to install in `/usr/local/include/`
cmake ..
# Or to install in the default system location for most Linux distros:
cmake -DCMAKE_INSTALL_PREFIX=/usr ..

sudo make install
```

## Usage

```cpp
// My library or source
#pragma once

#include <require/std/c++17>
// #include <require/std/gnu++11>
#include ...

```

## Authors and license

This library is written by [Stefan Hamminga](stefan@prjct.net) and may be freely shared, distributed and modified according to the terms of the Apache 2.0 license (included as the file `LICENSE`).

## Repository

[https://github.com/StefanHamminga/require](https://github.com/StefanHamminga/require)
