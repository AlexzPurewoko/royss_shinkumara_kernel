Patch using interdiff:

        interdiff -z patch-3.4.105 patch-3.4.106 | patch -p1
 

Build command:

-create file make_kernel.sh

-write in that file
        make <your config>
        make -j<number of your computer cores>

-command

        ./make_kernel.sh
 

Modules

        mkdir -p modules
        find . -name '*ko' -exec cp '{}' modules \;


Clean Source

        make clean
