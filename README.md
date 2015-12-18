Project Structure
=================
The mod loader currently consists of three projects:
- ModLoader: The core mod loader, outputs SpaarModLoader.dll
- ModLoader Injector: Used to create a patched Assembly-UnityScript.dll file that loads the mod loader
- ModLoader Installer: The Windows GUI installer

The file Patchset.txt contains all the modifications to Assembly-UnityScript.dll that have been made.

Building
========
A patched version of Assembly-UnityScript.dll, which is required for building is provided, as Besiege's modding conditions allow distribution of this file.
In order for Visual Studio to properly load the references and for the post-build step of installing the mod loader and the Start action to work, you will
need to set the BESIEGE_LOCATION environment variable to the path to your Besiege installation, including a \ at the end.

Futher information
==================
Check the README_enduser.md file for information about installing the mod loader and a list of features.