
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/67170c34-1d99-4e71-9e95-49f54ccde997/ddnhf6c-304fa073-814a-412d-a810-00d920e7e0b5.png/v1/fill/w_300,h_300/raspberry_pi_sticker_by_s_a_r_c_ddnhf6c-fullview.png?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9MzAwIiwicGF0aCI6IlwvZlwvNjcxNzBjMzQtMWQ5OS00ZTcxLTllOTUtNDlmNTRjY2RlOTk3XC9kZG5oZjZjLTMwNGZhMDczLTgxNGEtNDEyZC1hODEwLTAwZDkyMGU3ZTBiNS5wbmciLCJ3aWR0aCI6Ijw9MzAwIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmltYWdlLm9wZXJhdGlvbnMiXX0.LIDALUG5g_dTesR4k6QXHlIwCZK2EEcd8-PVN3KP5lk" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Life of [raspberry] Pi</h3>

  <p align="center">
    My (always evolving) MEGA-HOME-SERVER pi configuration
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About the Project</a></li>
    <li><a href="#prerequisites">Prerequisites</a></li>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>

<!-- About the Project -->

# About the Project
![Cover Image](images/cover_image.png)

This is my guide to setting up a raspberry pi home server that performs (but is not limited to) the following functions:
* Local file server
* Remote file server
* Plex Media Server
* Home VPN
* LAN Adblock
* Firewall
* Automated back-ups
* ... and then some

#### Why?
Every once in a while, an experiment blows up in my face and I end up spending a week getting everything back to normal,
because I never bothered noting down all the work as I'm doing it. This guide should serve as, both a record of all the 
configs, and possibly the start of some automated scripting-configing-recovery-ing-thingamajig.

<!-- GETTING STARTED -->
## Prerequisites

To get going, you need the following:
* A Raspberry Pi 🥧
  * Mine's a 4B. Technically, any [Pi model](https://support.plex.tv/articles/200375666-plex-media-server-requirements/) would do.
* A microSD Card ([min 32gb Class 10](https://www.tomshardware.com/best-picks/raspberry-pi-microsd-cards)) 💾
  * Get a good SD card, I've gone the cheaper route and that resulted in one of my reinstall-hell iterations
* A microSD Card Reader 💾
* Internet Access 🤷‍
* Wired or 2.4GHz USB Keyboard and Mouse 🖱️⌨️
  * [No wired keyboard / mouse?](./readmes/PIOS.md#dont-have-wired-keyboard--mouse-halp)
* Coffee ☕️

## Installation

* [Install and configure Pi OS](readmes/PIOS.md)
* [Setup File Sharing](readmes/SMB.md)
* [Install and configure Plex](readmes/Plex.md)
* [Set up auto backups](readmes/BackUP.md)

## Roadmap

- [x] Base piOS
- [x] Samba File Server
- [x] Plex Media Server
- [ ] Nord VPN
- [ ] PiHole DNS Sinkhole (Firewall & AdBlock)
- [x] Backups
- [ ] Jellyfin (opensource) Media Server
- [ ] Some other (opensource) VPN with mesh-net support
- [ ] Script base configurations

<!-- LICENSE -->
## License

Distributed under the GNU License. See [LICENSE.txt](LICENSE) for more information.
