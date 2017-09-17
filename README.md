# Reddit Enhancement Suite

Reddit Enhancement Suite (RES) is a suite of modules that enhances your Reddit browsing experience.

This is a fork of RES which will include backports of fixes as the official Safari version is now EOL.
Please check https://github.com/honestbleeps/Reddit-Enhancement-Suite for more details and licencing information.

## Building development versions of the extension

First time installation:

1. Install [git](https://git-scm.com/).
1. Install [node.js](https://nodejs.org) (version >= 6).
1. Install [Python 2](https://www.python.org/downloads/) (*not* version 3).
1. Navigate to your RES folder.
1. Run `npm install`.

Once done, you can build the extension by running `npm start`.

To load the extension into Safari, see below.

#### Details and advanced usage

**`npm run build [-- <browsers>]`** will clean `dist/`, then build RES (release mode). Each build output will be compressed to a .zip file in `dist/zip/`.

##### Building in Safari (assumes Mac)

  1. Open the `Preferences` by going to `Safari->Preferences` or pressing `⌘,`, then go to `Advanced` and check the checkbox for `Show Develop menu in menu bar`.
  2. Navigate to `Develop->Show Extension Builder` to open the extensions builder. Add a new extension by pressing the `+` in the bottom left and choosing `Add Extension`.
  3. Navigate to the `/dist/RES.safariextension` folder (not the `/safari` folder) for RES and select it.
  4. If you are using Safari 9+, you should be able to install the extension without enrolling in the [Apple Developer Program](https://developer.apple.com/programs/); however, the extension will be auto-uninstalled when you quit Safari.

  If you use an older version of Safari or find the auto-uninstall annoying, you need to purchase a proper certificate by signing up for the [Apple Developer Program](https://developer.apple.com/programs/) (currently $99/yr).