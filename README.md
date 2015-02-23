manifest
========

Local Manifest to build AOSP for the Sony Xperia Z3 (leo)

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the AOSP manifest
    
        repo init -u https://android.googlesource.com/platform/manifest -b android-5.0.2_r1

2. Add my local manifest

        mkdir .repo/local_manifests
        Copy sony.xml to .repo/local_manifests

3. Then sync up the repositories
 
        repo sync

4. Initialize the build environment

        source build/envsetup.sh && lunch
        
5. Select your device

6. Start building

        make –j <insert the cpu thread number of your computer>
  