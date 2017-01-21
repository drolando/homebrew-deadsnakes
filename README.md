# homebrew-deadsnakes

This formulae provide older versions of the Python package for OSX.

The formula in the homebrew official repository
only supports the latest version of Python 2 and Python 3, but people might still need to develop and test against 
these old Python interpreters. 

[![Build Status](https://travis-ci.org/drolando/homebrew-deadsnakes.svg)]
(https://travis-ci.org/drolando/homebrew-deadsnakes)

## How do I install these formulae?
Run `brew tap drolando/homebrew-deadsnakes` and then `brew install <formula>`

You can also install via URL:

``` bash
$ brew install https://raw.githubusercontent.com/drolando/homebrew-deadsnakes/master/Formula/<formula>.rb
```

## Usage

To install python 3.4:
``` bash
$ brew tap drolando/homebrew-deadsnakes
$ brew install python34
$ brew test python34
$ python3.4
Python 3.4.3 (default, Oct 20 2015, 22:36:21)
[GCC 4.2.1 Compatible Apple LLVM 7.0.0 (clang-700.0.72)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

To avoid messing with the official python version installed via homebrew, the binaries and libraries won't be
symlinked as `python`, `pip` or `wheel`. To use them you'll need to use their full name including the version.

``` bash
$ python3.3 --version
Python 3.3.6

$ pip3.3 list
pip (7.1.2)
setuptools (18.3.2)
wheel (0.26.0)

$ wheel3.3 version
wheel 0.26.0
```

## Supported Python Versions
Currently supported releases:

- 2.6
- 3.1
- 3.2
- 3.3
- 3.4

## Troubleshooting
First, please run `brew update` and `brew doctor`.

Second, read the [Troubleshooting Checklist]
(https://github.com/Homebrew/homebrew/blob/master/share/doc/homebrew/Troubleshooting.md#troubleshooting) 
and then [open an issue](https://github.com/drolando/homebrew-deadsnakes/issues/new) in this tap.
