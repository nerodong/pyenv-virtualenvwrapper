# pyenv-virtualenvwrapper

An [alternative approach](https://github.com/yyuu/pyenv-virtualenv) to manage virtualenvs from pyenv.

pyenv-virtualenvwrapper is a [pyenv](https://github.com/yyuu/pyenv) plugin
which provides an `pyenv virtualenvwrapper` command to manage your virtualenvs
with [virtualenvwrapper](http://pypi.python.org/pypi/virtualenvwrapper).

## Installation

### Installing python

Because virtualenvwrapper is depending on python, you must first install
at least one version of python.

For example, install `2.7.3` and set it as `global` in pyenv.

    $ pyenv install 2.7.3
    $ pyenv global 2.7.3

(NOTICE: virtualenvwrapper will not work if you remove the python version
which is bound to virtualenvwrapper.)

### Installing virtualenvwrapper

Installing virtualenvwrapper into your python.

    $ pip install virtualenvwrapper
    $ pyenv rehash

(NOTICE: if you have multiple python versions in pyenv, it is better to
install virtualenvwrapper into all the versions of python which you want
to work with virtualenvwrapper.)

### Installing pyenv-virtualenvwrapper as a pyenv plugin

Installing pyenv-virtualenvwrapper as a pyenv plugin will give you access to the
`pyenv virtualenvwrapper` and `pyenv virtualenvwrapper_lazy` command.

    $ mkdir -p ~/.pyenv/plugins
    $ cd ~/.pyenv/plugins
    $ git clone git://github.com/yyuu/pyenv-virtualenvwrapper.git

This will install the latest development version of pyenv-virtualenvwrapper into
the `~/.pyenv/plugins/pyenv-virtualenvwrapper` directory. From that directory, you
can check out a specific release tag. To update pyenv-virtualenvwrapper, run `git
pull` to download the latest changes.

## Usage

### Using `pyenv virtualenvwrapper`

To setup a virtualenvwrapper into your shell, just run `pyenv virtualenvwrapper`.
For example,

    $ pyenv virtualenvwrapper

or, if you favor `virtualenvwrapper_lazy.sh`,

    $ pyenv virtualenvwrapper_lazy

## Version History

#### 2013XXYY

 * Initial public release.

### License

(The MIT License)

* Copyright (c) 2013 Yamashita, Yuu

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.