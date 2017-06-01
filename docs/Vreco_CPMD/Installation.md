# Installation Procedure

## Obtaining the Code
Get the code from [GitHub](https://github.com/NNairIITK/Vreco_CPMD/)

```bash
git clone https://github.com/NNairIITK/Vreco_CPMD.git
```
**OR** use the SSH Key based url.

```bash
git clone git@github.com:NNairIITK/Vreco_CPMD.git
```

## Prerequisites
You'll need:

1. [Autotools](https://en.wikipedia.org/wiki/GNU_Build_System) [v. 2.68 minimum]
2. Some Fortran Compiler [most are supported, when in doubt, use [Gfortran](https://gcc.gnu.org/fortran/)]
3. [VMD](www.ks.uiuc.edu/Research/vmd/) [For visualization, optional]
4. [OPENDX](http://www.opendx.org/) [Also for visualization]

Autotools won't be needed for release candidates (RCs).

## Step-by-Step Breakdown
The following may be executed by typing them in blindly or by simply using the handy *copy* icon on the upper right of the HTML box.

These commands will work in any shell. [bash, zsh, fish etc.]

!!! Alert
	Readers are **strongly** urged to take some time out to understand the nature of the commands being typed out..

For preparing the RC setup:

```bash
aclocal
autoheader
autoconf
automake --add-missing
```

For end-user configuration and actual installation:

```bash
./configure
make
```

Configuration options are supported.
Make defaults to producing both **Vreco_CPMD.x** *and* **mtd_restart_extract.x**

## Options and Targets

TO-DO