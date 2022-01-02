gedit - Search triggered only after 3 letters are typedin 
============================================

project for fun  wont  completely work. will work on remaning part when god help me to do so .

when searching large log files, gedit hangs up when trying to type in commonly used words or letters vowels due large no of occurence


commit `0ff450dfec5a3530f308a2038f81e8a96559d06b` ignore searching if word is less than 3 letters

File: https://github.com/iamarjunsuresh/gedit-searchafter3letters/blob/9ec7af1229b33c8f3416159e6b109501aa8e395b/gedit/gedit-view-frame.c#L371

tweak above file  as per setting 


to install 
===
git clone </br>
cd gedit </br>
mkdir build </br>
cd build </br>
mkdir output </br>
meson --prefix=output/ </br>
ninja </br>
sudo ninja install  ( will overrwrite standard binary if prefix is not used) </br>


add custom prefix to  PATH & XDG_DATADIR if installed to custom prefix 

