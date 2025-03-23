# tofi-wifi-menu


<!-- GETTING STARTED -->
## Soo what is it?

A bash script that uses [tofi](https://github.com/philj56/tofi) to show available wifi networks, allows you to connect to them using nmcli and [zenity](https://gitlab.gnome.org/GNOME/zenity) for the password prompt.


## Prerequisites

You NEED these:

* [tofi](https://github.com/philj56/tofi)
* expect
* NetworkManager
* [zenity](https://gitlab.gnome.org/GNOME/zenity)


## Installation

* Clone the repo
   ```sh
   git clone https://github.com/soothsayerwally/tofi-wifi-menu.git
   ```

....and that's about it


## Usage

* Run the menu using
   ```sh
   ./tofi-wifi-menu.sh
   ```

### Stuff

Edit the included config to your will or just edit tofi-wifi-menu.sh to point to your existing tofi config. You might want to set a keybind for easy access

* Hyprland example: 
	add this to ~/.config/hypr/hyprland.conf
   ```
   bind = $mainMod, N, exec, /path-to/tofi-wifi-menu.sh
   ```


zenity uses gtk so to change how it looks, change your gtk theme using something like [nwg-look](https://github.com/nwg-piotr/nwg-look)


It takes some time for the password prompt to reappear if you enter a wrong password. DO NOT
PANIC.

<!-- How it looks -->
## How it looks


![A gif showing how it looks in action](tofi-wifi.gif)


<!-- ROADMAP -->
## Roadmap

- [ ] Handle open wifi networks
- [ ] Handle password prompt using just tofi (impossible?)
- [ ] QOL Features
	- [ ] Refresh button
	- [ ] wifi toggle

### Things you should know:
I don't know what I'm doing, so expect many bugs and don't expect me to ever fix them.
