Patching use interdiff

    interdiff -z patch-3.4.105 patch-3.4.106 | patch -p1
 
Build command

    ./make_kernel.sh
 
Clean Source

    make clean
 
Modules

    find . -name '*ko' -exec cp '{}' modules \;
