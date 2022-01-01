# Vocoder Plugin for DroidStar

This is an AMBE vocoder plugin based on mbelib and the OP25 AMBE encoder.  The makefiles create a shared object for various platforms that can be loaded via dlopen() (LoadLibrary on Windows).

# Compiling
All platforms require imbe_vocoder library be built and available for the platform being built.
The default Makefile is for a Linux PC.  MacOS can also use this file, just comment out the linux line and use the darwin line. The Makefile.win for windows requires a static mingw32 compiler.

# Builds
Location: http://pizzanbeer.net/plugins/

There are currently builds available for the following platforms:
- Linux 32-bit x86 platform:  vocoder_plugin.linux.i386
- Linux 64-bit x86 platform:  vocoder_plugin.linux.x86_64
- Linux 32-bit ARM platform (RaspiOS/Raspbian/etc): vocoder_plugin.linux.arm
- Linux 64-bit ARM platform (PINe64 PINEPHONE): vocoder_plugin.linux.arm64
- MacOS 64-bit x86 platform: vocoder_plugin.darwin.x86_64
- Windows 32-bit x86 platform: vocoder_plugin.winnt.i386
- Windows 64-bit x86 platform: vocoder_plugin.winnt.x86_64
- Android 32-bit ARM: vocoder_plugin.android.arm
- Android 64-bit ARM: vocoder_plugin.android.arm64
- IOS 32-bit ARM: vocoder_plugin.ios.arm
- IOS 64-bit ARM: vocoder_plugin.ios.arm64

Even though most RPis are arm64 architecture, the mainstream OS's are still 32 bit.

# Loading a plugin using the URL option (all devices)
- Visit the following link in your web browser: http://pizzanbeer.net/plugins/
- Press and hold the plugin for your device (arm or arm64)
- Select 'Copy link address' from the popup menu
- Open DroidStar and press and hold in the Vocoder URL field to paste the address
- Press 'Download vocoder'

# Manually loading of a plugin on Linux/MacOS/Windows
The settings location (where the settings file and host files reside are listed below.  You can manually place the plugin in this location.
- Linux: ~/.config/dudetronics
- MacOS: ~/.config/dudetronics
- Windows: C:/Users/<USER>/AppData/Local/<APPNAME> or C:/ProgramData/<APPNAME>


