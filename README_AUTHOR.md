Addon author instructions
================

This file contains instructions and explanations for you.
Bug reports are welcome, if you find errors in this template, or stuff doesn't work as expected.

These instructions are in part building upon the info to be found at http://ofxaddons.com/howto, so it's probably best if you go there and take a look first.

Addon name
----------
By convention, addons for openFrameworks begin with `ofx`, and follow camel-case capitalization, e.g. `myAwesomeNewAddon`.

Folder structure
----------------
The folder structure for an addon looks like this:

    of_preRelease/
      addons/
        addons_config.mk
        ofxMyAddon/
          docs/
              Doxyfile
              ...
          test/
              ...
          src/
            ofxMyAddon.h
            ofxMyAddon.cpp
            ...
          libs/
            necessaryLib/
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
          example_anExample/
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

Examples must have the string "example" in their folder name.
The OS folder names in `libs/necessaryLib/lib/` must not be changed.

Git repository
--------------
Probably the first thing you will want to do after downloading the template is rename the folder to your addon's name.
Then enter the folder, and create a git repository, e.g. by saying `git init` on the command line.

This template already contains a pre-made .gitignore file.
This file contains ignore patterns to prevent improper/irrelevant files from being 
committed to your git repository. 
If you find you have to force git to commit some files to your repository,
think about if you really should commit them, and if yes, adapt this file to your needs.

Since git does not keep track of empty directories, there are '.gitkeep' files in empty folders. 
You can safely remove them while developing your addon.

ofxaddons.com
-------------
At http://ofxaddons.com/ you will find a mostly automatically generated list of addons. When you publish your addon to Github, it will show up at this webpage after a couple of days or so.

Links
-----
Find more info on openframeworks at http://www.openframeworks.cc/
