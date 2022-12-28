# <img src="https://i.imgur.com/xUlg6lH.png" align="left" width="45" > elytraOS
*Let your Android experience fly.*

## Getting started
First of all, you should have a decent knowledge about the [Source Control Tools](https://source.android.com/setup/develop).

After you got all the needed commands for setting up your environment, set up the sources.

    repo init -u https://github.com/elytraOS/manifest.git -b tesseract

And then start syncing with our sources.

    repo sync --no-clone-bundle --current-branch --no-tags --force-sync -j$(nproc --all)

And now, you are ready to start building. Remember to set up device tree, common tree (if any) *etc*.

There are many way you can start to modify your device/common tree for building **elytraOS**. You can check our devices trees, if you have any problems. All of them (***should***) boot, and it's a great way of adapting your device tree to elytraOS.

## Building
Now that you (presumably) got everything working, you can finally start building elytraOS.

    . build/envsetup.sh
    lunch elytra_<codename>-userdebug
    make bacon -j32

## Credits
 * [**Paranoid Android**](https://github.com/AOSPA)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**CodeLinaro**](https://git.codelinaro.org/)
 * [**CodeAurora Forum**](https://source.codeaurora.org/quic/la)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**Project-Fluid**](https://github.com/Project-Fluid)
 * [**ProtonAOSP**](https://github.com/ProtonAOSP)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**ABC-ROM**](https://github.com/ezio84)
 * [**Yet another AOSP project**](https://github.com/Yaap)
 * [**Krypton Open Source Project**](https://github.com/Aosp-Krypton)
