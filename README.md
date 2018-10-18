### Ubuntu ftw!
## Instalación
* Arreglar el alt + tab https://askubuntu.com/a/996410/882392
* Instalar flatpak https://www.techrepublic.com/article/how-to-install-and-use-flatpak-on-ubuntu/
* Instalar chrome https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
* instalar hyper
* instalar vscode, sublime, intellij
* Instalar virtualbox https://www.virtualbox.org/wiki/Linux_Downloads
* Instalar ifconfig `sudo apt install net-tool`
* Instalar slack https://flathub.org/apps/details/com.slack.Slack
* instalar intellij con snap https://www.jetbrains.com/help/idea/install-and-set-up-product.html#install-on-linux-with-snaps

## Varios
* uso DD https://blog.kintoandar.com/2010/02/how-to-disk-dump-dd.html
    ```
    sudo dd if=backup_sda.img of=/dev/sdb bs=64k status=progress conv=fdatasync
    ```
* convertir imagne
    - https://superuser.com/questions/554862/how-to-convert-img-to-usable-virtualbox-format
    - 
* Limitar bandwidth https://www.tutorialspoint.com/articles/how-to-limit-network-bandwidth-on-linux
    ```
    sudo wondershaper wlp5s0 10000 500
    sudo wondershaper clear wlp5s0
    ```