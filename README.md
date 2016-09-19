# Перенос списка Debian пакетов с одного хоста на другой

## На исходном хосте

`dpkg --get-selections > INSTALLED`

## На целевом хосте
* `sudo dselect update`
* `sudo dpkg --clear-selections`
* `sudo dpkg --set-selections < INSTALLED`
* `sudo apt-get dselect-upgrade`
