Scorpion
------------------

Getting Started
------------------

To get started with building Scorpion Rom, you'll need to get familiar with Git and Repo.

Setting up the Build Environment:
Use this [Guide](https://raw.githubusercontent.com/nathanchance/Android-Tools/master/Guides/Building_AOSP.txt) as a reference for getting started

Initialize Source:

        mkdir scorpion (or whatever you want to name the source folder)

        cd ~/scorpion
        repo init -u https://github.com/ScorpionRom/scorpion_manifest.git -b sr-3.x

Sync Source:

        repo sync -c -j16 --force-sync --no-clone-bundle --no-tags

Build Source:

        . build/envsetup.sh
        lunch scorpion_crosshatch-userdebug (or whichever device you are building for, change out "crosshatch")
        make clean
        make bacon

Submitting Patches
------------------
We're open source, and patches are always welcome!

You can push to our Gerrit server: https://gerrit.scorpionrom.com


Credits:

Google for AOSP

Everyone at Dirty Unicorns

Ezio at ABC

Rinky McBally for our beloved logo

ROGERdotT (Roger Truttmann) for the v3.x wallpapers

Others we may have missed


