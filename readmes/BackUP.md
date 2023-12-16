# Auto Back-Ups

```shell
cd /Downloads
wget https://forums.raspberrypi.com/download/file.php?id=63044 my_tools.zip -O bkup_zip_name.zip
unzip bkup_zip_name -d ./bkup_folder_name
```

```shell
sudo sh ./image-backup -h  # help
sudo mkdir /media/some/backup/location/  # create a directory for storing backups
sudo bash image-backup -i /media/some/backup/location/back_name.img  # first back up
```

```shell
sudo crontab -e

```
[Crontab schedule expression editor](https://crontab.guru/#5_1_*_*_6)
```text
5 1 * * 6 sudo bash ~/path/to/image-backup/image-backup -i /media/path/to/backup/bkup.img >> /media/path/to/logs/bkup.log 2>&1
```