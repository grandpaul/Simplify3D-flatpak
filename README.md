
## Install Gnome Platform/SDK

 * flatpak remote-add --from gnome https://sdk.gnome.org/gnome.flatpakrepo
 * flatpak install gnome org.gnome.Platform//3.20
 * flatpak install gnome org.gnome.Sdk//3.20

## Build the package

 * Pay and download Simplify3D-3.1.1-linux-x64-installer.zip from the official
   site and put the zip together with the json file.
 * flatpak-builder --repo=mys3drepo simp1 simplify3d.json

## Add local repo

 * flatpak --user remote-add --no-gpg-verify mys3drepo mys3drepo

## Install the package

 * flatpak --user install mys3drepo com.ucrobotics.Simplify3D

## Update the package

 * flatpak --user update com.ucrobotics.Simplify3D

## Run the package

 * flatpak run com.ucrobotics.Simplify3D

 Note: you can also run it from the desktop launcher. We do provide a desktop
 file.
