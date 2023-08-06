# ptxconf
Pen tablet and Touch screen Xinput Configuration tool (PTXConf). Configures touch/pen devices to work with extended desktops and multiple screens on Linux.
Please find the installation and usage instructions in the documentation located here: [wenhsinjen.github.io/ptxconf/](http://wenhsinjen.github.io/ptxconf/)

WenHsin Linda Jen 2015

## Modifications introduced by Charlie Martínez in August 2023:

To create a Quirinux (and Debian 12) compatible .deb package I have modified the directory tree structure.

When testing the package, ptxconf.py was looking for the icon inside the user's /home, I modified this so that it also looks for it in /opt.

I have also changed the color of the icon, because it hardly contrasted in light themes. The color I chose works well for light as well as dark themes.

I also added autostart to /etc/xdg

## Dependences:

python3-full, gir1.2-appindicator3-0.1, python3-setuptools

## Documentation:

To work, this program needs the following dependencies:
python3-full, gir1.2-appindicator3-0.1, python3-setuptools

## Instalación / Release:
I accompany a successfully tested release on Debian 12, Sunday August 9, 2023.

To install on Debian 12, just run:

'apt install ./ptxconf_2.7_all.deb'

## Also available in the Quirinux repositories:

'apt-get update'
'apt-get install wget'

Create file /etc/apt/sources.list.d/quirinux.list with the following content:

'deb https://repo.quirinux.org quirinux main'

Then add the signature:

'wget -O - https://repo.quirinux.org/gpg/quirinux.asc | sudo apt-key add -'
'cd /etc/apt'
'sudo cp trusted.gpg trusted.gpg.d'

Finally, install:

'apt-get update'
'apt-get install ptxfonf'


