# <img src="https://i.imgur.com/xUlg6lH.png" align="left" width="45" > elytraOS
*Let your Android experience fly.*

## Getting started
First of all, you should have a decent knowledge about the [Source Control Tools](https://source.android.com/setup/develop).

After you got all the needed commands for setting up your environment, set up the sources.

    repo init -u git://github.com/elytraOS/manifest.git --depth=1

And then start syncing with our sources.

    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --current-branch

And now, you are ready to start building. Remember to set up device tree, common tree (if any) *etc*.

There are many way you can start to modify your device/common tree for building **elytraOS**. You can check our devices trees, if you have any problems. All of them (***should***) boot, and it's a great way of adapting your device tree to elytraOS.

## Building
Now that you (presumably) got everything working, you can finally start building elytraOS.

    . build/envsetup.sh
    lunch elytra_<codename>-userdebug
    brunch <codename>

#### Example
    . build/envsetup.sh
    lunch elytra_vayu-userdebug
    brunch vayu

### About bugs...
No one likes bugs. And some of them may be frustrating to fix. It's hard doing all alone, that's why we have our own chat for helping with your problem on Telegram! Join [here](https://t.me/elytraOSChat). 

We also recommend you to visit other groups on Telegram, like [@alaskalinuxuser_romdevelopment](https://t.me/alaskalinuxuser_romdevelopment) or [@AndroidBuildersHelp](https://t.me/AndroidBuildersHelp).

---
Now that you are ready for building and for releasing this amazing ROM, happy skydiving!
