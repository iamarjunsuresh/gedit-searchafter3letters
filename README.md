gedit - Search triggered only after 3 letters are typedin 
============================================

 
 
This is version 3.36.2 of gedit.

gedit is the official text editor of the GNOME desktop environment.
While aiming at simplicity and ease of use, gedit is a powerful general
purpose text editor.

Whether you are writing the next bestseller, programming an innovative
application, or simply taking some quick notes, gedit will be a reliable
tool to accomplish your task.

Its flexible plugin system allows you to tailor the application to your
 
 
=======
project for fun  wont  completely work. will work on remaning part when god help me to do so .
 

 
when searching large log files, gedit hangs up when trying to type in commonly used words or letters vowels due large no of occurence

 

commit `0ff450dfec5a3530f308a2038f81e8a96559d06b` ignore searching if word is less than 3 letters

File: https://github.com/iamarjunsuresh/gedit-searchafter3letters/blob/9ec7af1229b33c8f3416159e6b109501aa8e395b/gedit/gedit-view-frame.c#L371

tweak above file  as per setting 


to intall 

cd gedit 
mkdir build 
cd build
mkdir output 
meson --prefix=output/
ninja 
sudo ninja install  ( will overrwrite standard binary if prefix is not used)


setup XDG_DATADIR if installed to custom prefix 
 
To build gedit from source, see the [docs/build.md](docs/build.md) file.

How to report bugs
------------------

Please read
[the wiki page on how to report bugs](https://wiki.gnome.org/Apps/Gedit/ReportingBugs),
it contains a list of frequently reported bugs and a link to the bug
tracker.

Contributions
-------------

gedit development relies on voluntary contributions and everyone is invited
to help.

See the file [CONTRIBUTING.md](CONTRIBUTING.md) for more information.
 
