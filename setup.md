---
layout: page
title: setup
permalink: /setup/
---

{::comment}{:center: style="text-align: center"}{:/comment}
![xkcd_1168](https://imgs.xkcd.com/comics/tar.png)
{::comment}{:center}{:/comment}

# My work setup

There's a really great website called [Uses This][uses this] that asks people what they use to "get stuff done."  I love this idea of workflow transparency, so in the vein of sharing cool ideas, I hope this information will be useful to someone.

__Hardware__:  As of writing this (February 2018), I use a 2015 Macbook Air with an up-to-date OS and 8 GB of RAM.  It's a great little machine for plotting, but when I have to do any big data wrangling, I use supercomputers that live on the UC Irvine campus or in Wyoming.

__Storage__:  For peace of mind, I keep everything important on Dropbox, and I shell out money for the 1 TB per year option.  It's completely worth it.  My laptop was stolen in my 4th year of grad school, but thanks to cloud storage, I didn't lose a thing (well, except the computer itself).

## Software :floppy_disk:

__Terminal program:__ I'm on a terminal shell a lot, and my favorite text editor is [iTerm2][iterm2].  I like it because it allows for a lot more customization than the standard Terminal in Mac OS (the major selling point for me:  split panes!).

__Text editors:__ When I'm editing within terminal, I like vim, but my all-time favorite application-based text editor is the [BBEdit][bbedit] (I find the free version to be everything I need).  It's simple and, for me, a much more efficient alternative to vim.  I also like [Jupyter Notebook][jupyter] for Python.

__Color schemes:__ For color schemes, I like [Solarized][solarized], which was designed to be slightly easier on your eyes than the standard, pre-packaged options:  darks are less dark, whites are less white, but the contrast is still good.  I use the dark color scheme in iTerm2 and the light color scheme in BBEdit.

__Package mangers:__ To keep things clean and working on my Mac, I like to use the [Homebrew][homebrew] package manager.  It's great for keeping a lot of finicky dependencies in check, and I use it in conjunction with [conda][conda] (from the [Anaconda][anaconda] Python distribution).

## Language :snake:

In terms of data analysis, I'm a die-hard Python fan.  It was the first coding language I learned (circa 2008), and I'm a huge proponent of open-source software.

__Python distributions:__  My favorite way to keep the Python ecosystem on my computer healthy is [Anaconda][anaconda] (available for Mac, LINUX, and Windows).  I think it's the best way to install, use, and maintain a Python distribution.  The best part of Anaconda is that it can be installed in a user's home directory, and it doesn't require root permissions.  For me, this means I can create my own clean Python installation on _any_ computer I can log into, and I don't have to worry about having administrator privileges or dealing with dependency issues.

Another major selling point of Anaconda is that it allows me to maintain working environments of different Python versions and other goodies like NCO and CDO (see below).  In my experience, it's now easier than ever to have multiple, complex software programs installed and working happily on a single computer.  It's #neato.

__My favorite Python packages are__:

* [cartopy][cartopy] for making geo-referenced maps
* [pandas][pandas] for really simple manipulation of csv files and other common data formats
* [xarray][xarray] for a higher-dimensional version of pandas
* [wrf-python][wrf-python] for manipulating output from the Weather Research and Forecasting (WRF) model
* [netCDF4][netcdf4] for messing around with NetCDF files

## Useful tools for climate data analysis :earth_americas:

A few of my favorites include:

* [ncview][ncview]:  Written by David Pierce at Scripps, this is a really lightweight way to view NetCDF files.
* [NCO][nco]:  NCO stands for "NetCDF Operators" and has a few really great tools to splice up NetCDF files and do quick calculations on them (even regridding!).  [This website][jisao] out of the University of Washington has taught me everything I need to know.
* [CDO][cdo]:  CDO stands for Climate Data Operators, and this set of packages serves as a really great complement to NCO.
* [NCL][ncl]:  NCL is short for the NCAR Command Language, and this was developed by and for climate and weather scientists.  I find it a bit clunky as a language (it's unfortunately very similar to Fortran).  Still, it has a great support staff and a useful mailing list, and it's good at regridding and interpolating data if you're willing to summit the learning curve.

A final and useful fact:  NCO, CDO, and NCL can all be installed using conda, and homebrew can install ncview.  The days of annoying software dependencies are mostly over:  w:eyes:t!

[uses this]:https://usesthis.com/
[iterm2]:https://www.iterm2.com/
[conda]:https://conda.io/docs/
[solarized]:http://ethanschoonover.com/solarized
[bbedit]:https://www.barebones.com/products/bbedit/
[homebrew]:https://brew.sh/
[anaconda]:https://www.anaconda.com/download/
[jupyter]:http://jupyter.org/
[ncview]:http://meteora.ucsd.edu/~pierce/ncview_home_page.html
[nco]:http://nco.sourceforge.net/
[cdo]:https://code.mpimet.mpg.de/projects/cdo/
[jisao]:http://research.jisao.washington.edu/data_sets/nco/
[ncl]:https://www.ncl.ucar.edu/
[bbedit]:https://www.barebones.com/products/bbedit/
[cartopy]:http://scitools.org.uk/cartopy/
[pandas]:https://pandas.pydata.org/
[wrf-python]:http://wrf-python.readthedocs.io/en/latest/
[netcdf4]:http://unidata.github.io/netcdf4-python/
[xarray]:http://xarray.pydata.org/en/stable/