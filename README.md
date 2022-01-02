gedit - Search triggered only after 3 letters are typedin 
============================================

when searching large log files, gedit hangs up when trying to type in commonly used words or letters vowels due large no of occurence


commit is will ignore searching if word is less than 3 letters

File:
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

