# ofxAddonTemplate

This is an empty addon template for openframeworks.

Please read the info section to see how this
folder structure should be filled with your files!

## Installation

Download it here -> https://github.com/benben/ofxAddonTemplate/zipball/master
Unzip, rename and copy it to your addons folder

## Info

Since git does not keep track of empty directories, there are '.gitkeep' files in
empty folders. You can safely remove it while developing your addon.

The following explanation is stolen from http://ofxaddons.com/howto !
Head over to this side to get more info!

Folder structure for an addon looks like this:

    of_preRelease/
      addons/
        ofxMyAddon/
          src/
            ofxMyAddon.h
            ofxMyAddon.cpp
            ...
          libs/
            libwhatever/
              src/
                lib_implementation.h
                lib_implementation.cpp
                ...
              includes/
                libwhatever.h
                ...
              lib/
                osx/
                  static_libwhatever.a
                linux/
                  static_libwhatever.a
                ... //other platforms
          example-anExample/
            src/
              main.cpp
              testApp.h
              testApp.cpp
              ... //other source
            MyAddonExample.xcodeproj
            ... //other project files for other platforms
          bin/
            data/
              necessaryAsset.txt

## Links

For more info on openframeworks
-> http://www.openframeworks.cc/

For a list of addons and more info on addon development
-> http://ofxaddons.com/
