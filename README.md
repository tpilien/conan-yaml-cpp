[![Build Status](https://travis-ci.org/uilianries/conan-yaml-cpp.svg?branch=release/0.2.5)](https://travis-ci.org/uilianries/conan-yaml-cpp) [![Build status](https://ci.appveyor.com/api/projects/status/x0dv3a3l6koq8j3a/branch/release/0.2.5?svg=true)](https://ci.appveyor.com/project/uilianries/conan-yaml-cpp/branch/release/0.2.5) [![badge](https://img.shields.io/badge/conan.io-yaml--cpp%2F0.2.5-green.svg?logo=data:image/png;base64%2CiVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAMAAAAolt3jAAAA1VBMVEUAAABhlctjlstkl8tlmMtlmMxlmcxmmcxnmsxpnMxpnM1qnc1sn85voM91oM11oc1xotB2oc56pNF6pNJ2ptJ8ptJ8ptN9ptN8p9N5qNJ9p9N9p9R8qtOBqdSAqtOAqtR%2BrNSCrNJ/rdWDrNWCsNWCsNaJs9eLs9iRvNuVvdyVv9yXwd2Zwt6axN6dxt%2Bfx%2BChyeGiyuGjyuCjyuGly%2BGlzOKmzOGozuKoz%2BKqz%2BOq0OOv1OWw1OWw1eWx1eWy1uay1%2Baz1%2Baz1%2Bez2Oe02Oe12ee22ujUGwH3AAAAAXRSTlMAQObYZgAAAAFiS0dEAIgFHUgAAAAJcEhZcwAACxMAAAsTAQCanBgAAAAHdElNRQfgBQkREyOxFIh/AAAAiklEQVQI12NgAAMbOwY4sLZ2NtQ1coVKWNvoc/Eq8XDr2wB5Ig62ekza9vaOqpK2TpoMzOxaFtwqZua2Bm4makIM7OzMAjoaCqYuxooSUqJALjs7o4yVpbowvzSUy87KqSwmxQfnsrPISyFzWeWAXCkpMaBVIC4bmCsOdgiUKwh3JojLgAQ4ZCE0AMm2D29tZwe6AAAAAElFTkSuQmCC)](http://www.conan.io/source/yaml-cpp/0.2.5/uilianries/stable) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# A YAML parser and emitter in C++

[Conan.io](https://conan.io) package for [yaml-cpp](https://github.com/jbeder/yaml-cpp) project

The packages generated with this **conanfile** can be found in [conan.io](https://conan.io/source/yaml-cpp/0.2.5/uilianries/stable).

## Build packages

Download conan client from [Conan.io](https://conan.io) and run:

    $ python build.py

If your are in Windows you should run it from a VisualStudio console in order to get "mc.exe" in path.

## Upload packages to server

    $ conan upload yaml-cpp/0.2.5@uilianries/stable --all

## Reuse the packages

### Basic setup

    $ conan install yaml-cpp/0.2.5@uilianries/stable

### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*

    [requires]
    yaml-cpp/0.2.5@uilianries/stable

    [options]
    yaml-cpp:shared=True # False

    [generators]
    txt
    cmake

Complete the installation of requirements for your project running:</small></span>

    conan install .

Project setup installs the library (and all his dependencies) and generates the files *conanbuildinfo.txt* and *conanbuildinfo.cmake* with all the paths and variables that you need to link with your dependencies.

### License
[MIT](LICENSE)
