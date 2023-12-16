# Plex Media Server <img src="../images/Plex.png" style="height: 60px; vertical-align: middle">

## Pre-requisites
* [PIOS installed](../readmes/PIOS.md)
* [Static IP](../readmes/PIOS.md#some-more-configs)
* [Samba Share](../readmes/SMB.md) - if external drive sharing required, else [mount external drives](../readmes/SMB.md#auto-mount-at-startup)
## Instructions
* Update Pi
```shell
sudo apt-get update
sudo apt-get upgrade
```
## Install
```shell
sudo apt-get install apt-transport-https  # plex repos use https protocol, so enable that first
# Now, add the plex repos to apt's directory, and add official plex repo to sources list
curl https://downloads.plex.tv/plex-keys/PlexSign.key | gpg --dearmor | sudo tee /usr/share/keyrings/plex-archive-keyring.gpg >/dev/null
echo deb [signed-by=/usr/share/keyrings/plex-archive-keyring.gpg] https://downloads.plex.tv/repo/deb public main | sudo tee /etc/apt/sources.list.d/plexmediaserver.list
sudo apt-get update  # update once more
sudo apt-get install plexmediaserver  # actual install
```
## Configure
* In a browser, navigate to `YOUR_IP_ADDRESS:32400/web/`, and sign-in
* [Plenty of Tuts](https://support.plex.tv/articles/categories/plex-media-server/installation-and-basic-setup/) available
    for configurations