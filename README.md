# Git LFS X -- README
By spr
<!--@@VERSIONINC@@-->

## Introduction

Git LFS X contains the command line tool `git-lfs-x`, which adds functionality
that could perhaps be added to Git LFS.

## Windows

Use Ubuntu on Windows.  Do not use MSYS Git.

# Getting started

Initialize a Python 3 virtual environment to be used for `git-lfs-x` in the
sub-directory `local/venv` of the working copy:

On Linux, use a specific directory for the Linux release:

```bash
venvdir="venv-$(lsb_release -i -s)-$(lsb_release -r -s)" && echo "${venvdir}"
```

Otherwise use a generic directory:

```bash
venvdir=venv
```

```bash
python3 -m venv local/${venvdir}
 # or
virtualenv -p python3 local/${venvdir}
```

```bash
./local/${venvdir}/bin/pip3 install -r requirements.txt
```

To run Git LFS X:

```bash
./bin/git-lfs-x --help
```
