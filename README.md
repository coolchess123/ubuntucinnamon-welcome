Cinnamon Welcome
==============

Welcome screen application to greet new users on their first login.

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-white.svg)](https://snapcraft.io/ubuntu-ubuntucinnamon-welcome)

### Translators

We need to translate ubuntucinnamon-welcome into your language/locale.  Please
help-out - visit:

https://www.transifex.com/ubuntu-cinnamon/ubuntucinnamon-welcome/

### Installation

```sh
sudo apt install gir1.2-webkit2-4.0 python3-notify2 node-uglify
git clone https://github.com/Ubuntu-Cinnamon-Remix/ubuntucinnamon-welcome.git

uglifyjs -o data/js/bootstrap.min.js data/js/bootstrap.js
uglifyjs -o data/js/baguetteBox.min.js data/js/baguetteBox.js
uglifyjs -o data/js/popper.min.js data/js/popper.js
```

### Testing

```sh
cd ubuntucinnamon-welcome
./ubuntucinnamon-welcome -d
```

To test the live session

    ./ubuntucinnamon-welcome --force-session=live -d
    
To test a language or locale

    ./ubuntucinnamon-welcome --locale=pl
    
change "pl" to your language i18n shortcode

### Compile scss files
```sh
 ./sassc-compile.sh
```

### Screenshot
#### Live session
![Screenshot of Cinnamon Remix Welcome App](https://raw.githubusercontent.com/cinnamon-remix/ubuntucinnamon-welcome/master/screenshot-live-session.png)

#### Normal session
![Screenshot of Cinnamon Remix Welcome App](https://raw.githubusercontent.com/cinnamon-remix/ubuntucinnamon-welcome/master/screenshot-normal-session.png)

### LICENSES
  The project contains files with a variety of licenses.
  For the complete list of licenses, see [debian/copyright](https://github.com/cinnamon-remix/ubuntucinnamon-welcome/blob/master/debian/copyright) file.
