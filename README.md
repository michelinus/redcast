# Redcast

Redcast is a SEGA Dreamcast emulator written in C.

![Screenshot](https://dumpshare.net/images/3365307software.png)

## Code Status: [![Build status](https://ci.appveyor.com/api/projects/status/5r334cx8b114e56c?svg=true)](https://ci.appveyor.com/project/michelinus/redream)
 
## Tasks list
- [x] Add a button for the boot of the Dreamcast BIOS in the System tab.)
- [x] Enable disabled mouse in full screen GUI and disable it in-game only.
- [x] Reorganize the vital files of the application to allow the output in the folder of the EXE file.
- [ ] Insert a "break" function to change game (in this state you need to reopen the software).
- [ ] Changing the interface from blue to red color.
- [ ] Adding more languages, prioritizing Italian.
 
## Building
- Clone this repository and create a `build` directory
   - Generate a makefile for your OS
   ```
   # Makefile Linux
   cmake -DCMAKE_BUILD_TYPE=RELEASE ..
   # Xcode project
   cmake -G "Xcode" ..
   # Visual Studio project
   cmake -G "Visual Studio 15 Win64" ..
   ```

     - Run `make` from the command line if you've generated a `Makefile`
       - Or load up the project file and compile the code from inside of your IDE.

## Credits
Basically all the work was done by [redream](https://github.com/inolen/redream) by inolen.

## License
Redream is licensed under the GPLv3 license.
It uses third party libraries that are each distributed under their own terms (see each library's license in deps).