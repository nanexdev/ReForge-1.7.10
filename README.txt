README: Reforge (Minecraft 1.7.10)

Welcome to Reforge, a modernized fork of the Minecraft Forge 10.13.4.1614 build for Minecraft 1.7.10. Reforge aims to breathe new life into the 1.7.10 ecosystem by providing the performance enhancements and stability fixes required by modern hardware and complex modpacks.

Reforge is an unofficial, high-performance fork of the original Forge project. While it maintains 100% compatibility with existing 1.7.10 Forge mods, it replaces the aging internal logic with modern optimizations found in newer versions of Minecraft and standalone performance mods.
Key Features:

    Modern Rendering Pipeline: Backports logic from modern rendering engines to reduce CPU overhead.

    Asynchronous Multi-threading: Moves chunk loading and data processing to background threads, significantly reducing "world lag" and TPS spikes.

    Enhanced Fullscreen Handling: Replaces the buggy legacy fullscreen mode with a stable, modern implementation that supports Borderless Windowed mode and prevents crashing when ALT+TABbing.

    Optimized Atlas Stitching: Improves the way textures are compiled into the game’s sprite sheets (atlases), reducing RAM usage and decreasing initial loading times for heavy modpacks.

    Modern Java Support: Provides better out-of-the-box compatibility with Java 8 (latest builds) and experimental support for newer JDKs.

    Built-in Mixin Support: Includes a native Mixin bootstrap to ensure compatibility with modern performance mods like Angelica or FalseTweaks.

*** HOW TO INSTALL ***
For Mod Users:

Download the latest installer from http://files.minecraftforge.net and follow instructions given by the installer.


For Mod Devs:

Download the latest Forge source distribution from http://files.minecraftforge.net and unzip it to a folder.
Open a command prompt, navigate to the directory where you unzipped the Forge sources, and run:
If you have Gradle: gradle setupDevWorkspace
If you DO NOT have Gradle installed:
Windows: ./gradlew.bat setupDevWorkspace
MacOS/Linux: ./gradlew setupDevWorkspace

If you wish to use the Eclipse IDE, run gradle eclipse instead of gradle setupDevWorkspace, or install the Gradle plugin for Eclipse and import the Forge source folder as a Gradle project.

To get the decompiled classes:
If you have Gradle: gradle setupDecompWorkspace
If you DO NOT have Gradle installed:
Windows: ./gradlew.bat setupDecompWorkspace
MacOS/Linux: ./gradlew setupDecompWorkspace

For Contributors: (Note: This assumes you have Gradle installed. If you don't, use ./gradlew(.bat) instead of gradle.

Clone this repository to a folder. 
Open a command prompt and navigate to the folder where you cloned this repo.
Run gradle setupForge to setup your development environment.

To use Eclipse, point your Eclipse workspace at the eclipse folder inside the repo.


Requirements (for both mod devs and contributors):
  You must have a JDK installed and accessible.
  If you do not wish to use the gradle wrapper, you can install Gradle from http://www.gradle.org/ .
 
