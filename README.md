# Pulverizr

Pulverizr will smash your images down to size. It uses a number of free, and often times open source, programs to optimize and compress image files while still retaining their original appearance.

## Dependencies

If you're on Ubuntu, almost all of these dependencies can be retrieved using **apt**. Although Pulverizr works best with all its dependencies, 

* [gifsicle](http://www.lcdf.org/gifsicle/) 1.58+
* [libjpeg](http://www.ijg.org/) (or **libjpeg-progs** if you're using **apt**)
* [node](http://nodejs.org/) v0.1.95+
* [node-promse](http://github.com/kriszyp/node-promise) (**included**)
* [optipng](http://optipng.sourceforge.net/) 0.6.3+
* [pngcrush](http://pmt.sourceforge.net/pngcrush/) 1.7.0+

### On Mac OSX

**Coming soon!**

### On Ubuntu

To install the dependencies on Ubuntu:

    sudo apt-get install gifsicle libjpeg-progs optipng pngcrush

### On Windows

Good luck to you, sir.

## Installation

First you'll need to make sure all git submodules have been downloaded. To do this, simply run:

    make

Once you have all the submodules, install Pulverizr to **/usr/local/bin** by running:

    make install

## Usage

Since I'm too lazy right now to go through everything in detail, here's what you'll see if you run "**pulverize -h**".

    Usage: pulverize [OPTION]... [FILE]...
    Smash your images down to size. Pulverizr uses several compressors/optimizers
    to squeeze every last bit out of your images. If Pulverizr detects an
    optimization, it overwrites the old image with the newly optimized one.

    Options:

     General:
      -a, --aggressive	uses more aggressive compression algorithms (takes longer, 
    			works better)
      --dry-run		print summary but don't actually modify files
      -q, --quiet		pulverizer will stfu
      --verbose		verbose mode

     Traversing:
      -R, --recursive	scan directories recursively

     Other:
      -h, --help		print this handy dandy help page
      -v, --version		print program version

## Special Thanks

See **Dependencies**
