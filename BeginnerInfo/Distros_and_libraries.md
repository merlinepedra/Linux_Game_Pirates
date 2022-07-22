# Distros and libraries - BeginnerInfo

I will be providing some recommendations here. Take into consideration that this is based on my own opinions and experience. Others may contribute to information here in time.

## Distros

I recommend using Arch based distros or Arch itself, in which case, what are you here for?

* There are a few reasons for it:

1. You have up-to-date drivers and software which is necessary for a gaming-focused system.
2. The dependency system is easier to manage vs distros like Ubuntu/PopOS and so on.
3. Using certain wine builds like TKG requires up-to-date version of `glibc`, which Ubuntu for example doesn't have.
4. You can use repositories like chaotic-aur which proivdes up to date, precompiled builds that are necessary to play or test games. Some of those are:
```sh
mesa-devel, wine-tkg, proton-tkg, vkd3d-tkg, linux-tkg, linux-xanmod, nvidia-dev drivers and so on.
```
5. Arch is just better. :)
------------------------------------------------------------------------------------------------------------------

* Arch based distros:
1. `Garuda` - Comes with chaotic-aur and linux-zen by default, updates for it come precompiled. This enables fsync support and other performance improvements. You need to install pamac manually.
2. `ArcoLinux` - While it doesn't come with default improvements like the above, it is ok.
3. `EndeavourOS` - It may be more trusted than Manjaro but the experience is kinda clunky, at least in my experience.
4. `Manjaro` - Not trusted anymore by the community as it fails to maintain and provide proper support. You're better off getting updates directly from Arch like Garuda and ArcoLinux does.
5. `KaOS`

## Drivers and libraries

- I'm only going to mention packages for Arch as I have already explained my reasoning.

You should have these drivers installed:<br>

***AMD*** drivers:
```sh
lib32-mesa vulkan-radeon lib32-vulkan-radeon vulkan-icd-loader lib32-vulkan-icd-loader
```

***Nvidia*** drivers:
```sh
nvidia-dkms nvidia-utils lib32-nvidia-utils nvidia-settings vulkan-icd-loader lib32-vulkan-icd-loader
```

***Intel*** drivers:
```sh
lib32-mesa vulkan-intel lib32-vulkan-intel vulkan-icd-loader lib32-vulkan-icd-loader
```
------------------------------------------------------------------------------------------------------------------
* Native games:
- `GOG` Native games come with runtime included, which means it shouldn't have problems with missing libraries.
- Steam has `Steam-Runtime` builtin on it's client and is not included in the game files. I have built a [script](http://it7otdanqu7ktntxzm427cba6i53w6wlanlh23v5i3siqmos47pzhvyd.onion/johncena141/Linux_Game_Pirates/src/branch/master/Tools/Runtime-Installer) that easily adds steam runtime and creates start script.
- Having Steam installed should also provide some useful libraries.

* Wine games:
1. For my uploads as example, you need wine installed on your system even if wine is already provided in the torrent, because it needs the dependencies.
2. Having Steam installed should also provide some useful libraries.

# Contributors
```
johncena141
```