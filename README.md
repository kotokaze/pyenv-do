# pyenv-do

pyenv-do is a [pyenv](https://github.com/pyenv/pyenv) plugin
that provides a `pyenv do` command to exeute command installed in pyenv-managed Python.
This is the improvement of original `pyenv exec` command.
(See also issue [#1932](https://github.com/pyenv/pyenv/issues/1932))

## Installation

### Installing as a pyenv plugin

Installing pyenv-do as a pyenv plugin will give you access to the `pyenv do` command.

    $ git clone https://github.com/kotokaze/pyenv-do.git $(pyenv root)/plugins/pyenv-do

## Usage

To execute in a specific version, just start with `pyenv do --env <version>`.

    $ pyenv do --env 3.8.13 python --version
    Python 3.8.13

Or, you can use instead of the `pyenv exec` command (current version will be used).

    $ pyenv do pip install -r requirements.txt

## Version History

#### 20221005

 * Initial public release.
