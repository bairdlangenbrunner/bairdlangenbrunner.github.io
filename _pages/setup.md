---
title: " "
layout: single
permalink: /setup/
header:
  overlay_image: 
---

{:center: style="text-align: center"}
![xkcd_1168](https://imgs.xkcd.com/comics/tar.png)
{:center}

# My work setup

There's a really great website called [Uses This][uses this] that asks people what they use to "get stuff done."  I love this idea of workflow transparency, so in the vein of sharing cool ideas, I hope this information will be useful to someone.

<hr>

__Hardware__:  I use a Macbook Air (2015) with an up-to-date OS and 8 GB of RAM.  It's a great little machine for plotting, but when I have to do any big data wrangling, I use supercomputers that live on the UC Irvine campus or in Wyoming.

__Storage__:  For peace of mind, I keep everything important on Dropbox, and I shell out money for the 1 TB per year option.  It's completely worth it.  My laptop was stolen in my 4th year of grad school, but thanks to cloud storage, I didn't lose a thing (well, except the computer itself).

## Software

I'm on a terminal shell a lot, and my favorite text editor is [iTerm2][iterm2].  I like it because it allows for a lot more customization than the standard Terminal in Mac OS.  I can also use split panes, which was one of the reasons I switched over.

When I'm editing in terminal, I tend to use standard UNIX vi, but I find it fairly exhausting after a while.  My all-time favorite text editor is the __free__ version of [BBEdit][bbedit].  It's simple to use, you can add language-specific syntax highlighting.  After the 30-day trial, you can still use most of the features.

For color schemes, I like [Solarized][solarized], which was designed to be slightly easier on your eyes than the standard, pre-packaged options:  darks are less dark, whites are less white, but the contrast is still good.  I use the dark color scheme in iTerm2 and the light color scheme in BBEdit.

To keep things clean and working on my Mac, I like to use the [Homebrew][homebrew] package manager.  It's great for keeping all of those finicky dependencies in check, and I can even install a language specific to the climate modeling community.

## Languages

Where coding is concerned, I'm a die-hard Python fan.  It was the first coding language I ever learned (circa 2008), and I'm a huge proponent of open-source software.  I prefer Python 3.

My favorite way to keep Python working on my computer is via [Anaconda][anaconda] (available for Mac, LINUX, and Windows).  I think it's the best way to install, use, and maintain a Python.  The best part of Anaconda is that it can be installed in a user's home directory, and it doesn't require root permissions.  For me, this means I can create my own clean Python installation on any computer I can log into, and I don't have to worry about having administrator privileges and dealing with dependency issues.

The editor I write Python code in is typically either BBEdit (for .py scripts that I'm using to do heavy calculations) or [Jupyter][jupyter] Notebooks (for exploratory analysis and to fine-tune plots).

My favorite Python packages are:
* The Matplotlib [Basemap Toolkit][] for making geo-referenced maps
* [pandas][] for really simple manipulation of csv files and other common data formats
* [wrf-python][] for manipulating output from the Weather Research and Forecasting (WRF) model
* [netCDF4][] for manipulating NetCDF files

## Useful tools for climate data analysis

A few of my favorites include:

* [ncview][ncview]:  Written by David Pierce at Scripps, this is a really lightweight way to view NetCDF files.
* [NCO][nco]:  NCO stands for "NetCDF Operators" and has a few really great tools to splice up NetCDF files and do quick calculations on them.  [This website][jisao] out of the University of Washington has taught me everything I need to know.
* [CDO][cdo]:  CDO means Climate Data Operators, and this set of packages serves as a really great complement to NCO.
* [NCL][ncl]:  NCL is short for the NCAR Command Language, and this was developed by and for climate and weather scientists.  I find it a bit clunky as a language (it's unfortunately very similar to Fortran), but it does some things really well:  regridding climate data, interpolating to pressure levels, etc.  It also has a great support staff and a useful mailing list.

A final and useful fact:  ncview, NCO, and CDO can all be installed using Homebrew.  NCL you'll have to install from source (but the website has good instructions).

[uses this]:https://usesthis.com/
[iterm2]:https://www.iterm2.com/
[solarized]:http://ethanschoonover.com/solarized
[bbedit]:https://www.barebones.com/products/bbedit/
[homebrew]:https://brew.sh/
[anaconda]:https://www.anaconda.com/download/
[jupyter]:http://jupyter.org/
[ncview]:http://meteora.ucsd.edu/~pierce/ncview_home_page.html]
[nco]:http://nco.sourceforge.net/
[cdo]:https://code.mpimet.mpg.de/projects/cdo/
[jisao]:http://research.jisao.washington.edu/data_sets/nco/
[ncl]:https://www.ncl.ucar.edu/
