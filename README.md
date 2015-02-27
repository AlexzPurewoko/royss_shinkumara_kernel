Patch using interdiff:

        interdiff -z <your old patch> <your new patch> | patch -p1
 

Build command:

-create file make_kernel.sh

-write in that file

        make <your config>
        make -j<number of your computer cpu cores>

-command

        ./make_kernel.sh
 

Modules

        mkdir -p modules
        find . -name '*ko' -exec cp '{}' modules \;


Clean Source

        make clean
