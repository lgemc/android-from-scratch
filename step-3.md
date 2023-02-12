## Installing android emulator

To get android emulator working, first we need to install system image

## Android system images format

If you take a look on `sdkmanager --list` output you can find that outputs are like this

`system-images;android-33;google_apis_playstore;arm64-v8a`

And, what it means?

*system-images*: It means that the development package is a prebuilt version of android
*android-33*: is the version release, is a little strange that you will not find android 7 (nougat) or android 11, this is because
this versioning is an public image build version, you can see that as a 12.x or 5.x release version.

For example, android 33 image corresponds with android 13 major version.

*google_apis*: android operative system version to install
Available options here:
- google_apis: explained above
- google_apis_playstore: android, with playstore
- google-tv
- android-tv
- android-wear

By now we will pick *google_apis*

*x86_64*: means that image was build to work in desktop cpu compatible with 64 bits instruction set
Available options here:
- x86_64
- arm64-v8a
- x86
Install it with `sdkmanager --install 'system-images;android-33;google_apis;arm64-v8a'`

After that we have a prebuild `android image` and `android emulator`, next step you will see it in action.
