# color_util

A lightweight, header-only C++ utility library for adding ANSI escape colors to terminal output.

## Features

* **Header-only**: Just include `color_util.hpp` and you are good to go. No compilation required.
* **Highly Compatible**: Supports **C++98 or later**.
* **Zero Dependencies**: Pure standard C++ without any external overhead.

## Usage

Simply stream the constants from the `Kumalib::color` namespace to `std::cout`. 
Always remember to use `reset` to restore the default terminal color.

```cpp
#include <iostream>
#include "color_util.hpp"

int main() {
    std::cout << Kumalib::color::red     << "This is Red"     << Kumalib::color::reset << std::endl;
    std::cout << Kumalib::color::green   << "This is Green"   << Kumalib::color::reset << std::endl;
    std::cout << Kumalib::color::yellow  << "This is Yellow"  << Kumalib::color::reset << std::endl;
    std::cout << Kumalib::color::blue    << "This is Blue"    << Kumalib::color::reset << std::endl;
    std::cout << Kumalib::color::magenta << "This is Magenta" << Kumalib::color::reset << std::endl;
    std::cout << Kumalib::color::cyan    << "This is Cyan"    << Kumalib::color::reset << std::endl;

    return 0;
}