
* Fetch sources
```
repo init -u https://android.googlesource.com/platform/manifest android-5.1.1_r36
repo sync -j8
```

* Install these dependencies (Ubuntu 15.10)
```
sudo apt-get update
sudo apt-get install openjdk-8-jdk
```
```
sudo apt-get install git-core gnupg flex bison gperf build-essential \
  zip curl zlib1g-dev gcc-multilib g++-multilib libc6-dev-i386 \
  lib32ncurses5-dev x11proto-core-dev libx11-dev lib32z-dev ccache \
  libgl1-mesa-dev libxml2-utils xsltproc unzip
```

* source build/envsetup.sh
* lunch
* make -j16
* emulator &

NOTE:

If you face below error

```
You have tried to change the API from what has been previously approved.

To make these errors go away, you have two choices:
   1) You can add "@hide" javadoc comments to the methods, etc. listed in the
      errors above.

   2) You can update current.txt by executing the following command:
         make update-api

      To submit the revised current.txt to the main Android repository,
      you will need approval.
```

then execute this

* make update-api

* make -j16

* emulator &
