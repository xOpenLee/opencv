###toolchain.cmake
# this one is important
set( CMAKE_SYSTEM_NAME Linux )

#this one not so much
set( CMAKE_SYSTEM_PROCESSOR arm )

# specify the cross compiler
set( CMAKE_C_COMPILER /opt/freescale/usr/local/gcc-4.6.2-glibc-2.13-linaro-multilib-2011.12/fsl-linaro-toolchain/bin/arm-none-linux-gnueabi-gcc )
set( CMAKE_CXX_COMPILER /opt/freescale/usr/local/gcc-4.6.2-glibc-2.13-linaro-multilib-2011.12/fsl-linaro-toolchain/bin/arm-none-linux-gnueabi-g++ )

# where is the target environment - point to your rootfs here
set( CMAKE_FIND_ROOT_PATH  /home/xopenlee/proj/ltib/rootfs )

# search for programs in the build host directories
set( CMAKE_FIND_ROOT_PATH_MODE_PROGRAM NEVER )

# for libraries and headers in the target directories
set( CMAKE_FIND_ROOT_PATH_MODE_LIBRARY ONLY )
set( CMAKE_FIND_ROOT_PATH_MODE_INCLUDE ONLY )

# point to your rootfs path here 
set( CMAKE_CXX_FLAGS "-L/home/xopenlee/proj/ltib/rootfs/usr/lib" )

