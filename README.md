vladimir@Acer2010:~$ sudo su
[sudo] пароль для vladimir: 
root@Acer2010:/home/vladimir# cd ..
root@Acer2010:/home# cd..
cd..: команда не найдена
root@Acer2010:/home# cd ..
root@Acer2010:/# mkdir -p ./test/folder
root@Acer2010:/# nano ./test/folder/test.txt
root@Acer2010:/# nano ./test.txt
root@Acer2010:/# ls
0     cdrom  home   lib64       media  proc  sbin  swapfile  test.txt  var
bin   dev    lib    libx32      mnt    root  snap  sys       tmp
boot  etc    lib32  lost+found  opt    run   srv   test      usr
root@Acer2010:/# sudo docker run -it -h DJC --name djc_test -v /test/folder:/otherway -v /root/test.txt:/otherway/test.txt ubuntu:22.10
sudo: docker: команда не найдена
root@Acer2010:/# sudo apt update
Пол:1 http://security.ubuntu.com/ubuntu jammy-security InRelease [110 kB]      
Сущ:2 http://ru.archive.ubuntu.com/ubuntu jammy InRelease                      
Пол:3 http://ru.archive.ubuntu.com/ubuntu jammy-updates InRelease [119 kB] 
Пол:4 http://ru.archive.ubuntu.com/ubuntu jammy-backports InRelease [108 kB]
Получено 337 kB за 5с (61,4 kB/s)         
Чтение списков пакетов… Готово
Построение дерева зависимостей… Готово
Чтение информации о состоянии… Готово         
Может быть обновлено 3 пакета. Запустите «apt list --upgradable» для их показа.
root@Acer2010:/# sudo apt upgrade
Чтение списков пакетов… Готово
Построение дерева зависимостей… Готово
Чтение информации о состоянии… Готово         
Расчёт обновлений… Готово
Следующие пакеты устанавливались автоматически и больше не требуются:
  libflashrom1 libftdi1-2
Для их удаления используйте «sudo apt autoremove».
Get more security updates through Ubuntu Pro with 'esm-apps' enabled:
  libvlc5 vlc-data libvlccore9 libpostproc55 libavcodec58 libavutil56
  libswscale5 libswresample3 vlc-plugin-video-output libavformat58 libvlc-bin
  vlc-plugin-base libavfilter7
Learn more about Ubuntu Pro at https://ubuntu.com/pro
#
# An OpenSSL vulnerability has recently been fixed with USN-6188-1 & 6119-1:
# CVE-2023-2650: possible DoS translating ASN.1 object identifiers.
# Ensure you have updated the package to its latest version.
#
Следующие пакеты будут оставлены в неизменном виде:
  gjs gnome-remote-desktop libgjs0g
Обновлено 0 пакетов, установлено 0 новых пакетов, для удаления отмечено 0 пакетов, и 3 пакетов не обновлено.
root@Acer2010:/# sudo apt install docker -y
Чтение списков пакетов… Готово
Построение дерева зависимостей… Готово
Чтение информации о состоянии… Готово         
Следующие пакеты устанавливались автоматически и больше не требуются:
  libflashrom1 libftdi1-2
Для их удаления используйте «sudo apt autoremove».
Будут установлены следующие дополнительные пакеты:
  wmdocker
Следующие НОВЫЕ пакеты будут установлены:
  docker wmdocker
Обновлено 0 пакетов, установлено 2 новых пакетов, для удаления отмечено 0 пакетов, и 3 пакетов не обновлено.
Необходимо скачать 14,3 kB архивов.
После данной операции объём занятого дискового пространства возрастёт на 58,4 kB.
Пол:1 http://ru.archive.ubuntu.com/ubuntu jammy/universe amd64 wmdocker amd64 1.5-2 [13,0 kB]
Пол:2 http://ru.archive.ubuntu.com/ubuntu jammy/universe amd64 docker all 1.5-2 [1 316 B]
Получено 14,3 kB за 0с (49,0 kB/s)    
Выбор ранее не выбранного пакета wmdocker.
(Чтение базы данных … на данный момент установлено 218739 файлов и каталогов.)
Подготовка к распаковке …/wmdocker_1.5-2_amd64.deb …
Распаковывается wmdocker (1.5-2) …
Выбор ранее не выбранного пакета docker.
Подготовка к распаковке …/archives/docker_1.5-2_all.deb …
Распаковывается docker (1.5-2) …
Настраивается пакет wmdocker (1.5-2) …
Настраивается пакет docker (1.5-2) …
Обрабатываются триггеры для man-db (2.10.2-1) …
root@Acer2010:/# sudo apt install docker.io -y
Чтение списков пакетов… Готово
Построение дерева зависимостей… Готово
Чтение информации о состоянии… Готово         
Следующие пакеты устанавливались автоматически и больше не требуются:
  libflashrom1 libftdi1-2
Для их удаления используйте «sudo apt autoremove».
Будут установлены следующие дополнительные пакеты:
  containerd pigz runc ubuntu-fan
Предлагаемые пакеты:
  aufs-tools btrfs-progs cgroupfs-mount | cgroup-lite debootstrap docker-doc
  rinse zfs-fuse | zfsutils
Следующие НОВЫЕ пакеты будут установлены:
  containerd docker.io pigz runc ubuntu-fan
Обновлено 0 пакетов, установлено 5 новых пакетов, для удаления отмечено 0 пакетов, и 3 пакетов не обновлено.
Необходимо скачать 72,0 MB архивов.
После данной операции объём занятого дискового пространства возрастёт на 286 MB.
Пол:1 http://ru.archive.ubuntu.com/ubuntu jammy/universe amd64 pigz amd64 2.6-1 [63,6 kB]
Пол:2 http://ru.archive.ubuntu.com/ubuntu jammy-updates/main amd64 runc amd64 1.1.4-0ubuntu1~22.04.3 [4 244 kB]
Пол:3 http://ru.archive.ubuntu.com/ubuntu jammy-updates/main amd64 containerd amd64 1.6.12-0ubuntu1~22.04.3 [34,4 MB]                        
Пол:4 http://ru.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 docker.io amd64 20.10.21-0ubuntu1~22.04.3 [33,3 MB]                   
Пол:5 http://ru.archive.ubuntu.com/ubuntu jammy/universe amd64 ubuntu-fan all 0.12.16 [35,2 kB]                                              
Получено 72,0 MB за 4мин 57с (243 kB/s)                                                                                                      
Предварительная настройка пакетов …
Выбор ранее не выбранного пакета pigz.
(Чтение базы данных … на данный момент установлено 218749 файлов и каталогов.)
Подготовка к распаковке …/archives/pigz_2.6-1_amd64.deb …
Распаковывается pigz (2.6-1) …
Выбор ранее не выбранного пакета runc.
Подготовка к распаковке …/runc_1.1.4-0ubuntu1~22.04.3_amd64.deb …
Распаковывается runc (1.1.4-0ubuntu1~22.04.3) …
Выбор ранее не выбранного пакета containerd.
Подготовка к распаковке …/containerd_1.6.12-0ubuntu1~22.04.3_amd64.deb …
Распаковывается containerd (1.6.12-0ubuntu1~22.04.3) …
Выбор ранее не выбранного пакета docker.io.
Подготовка к распаковке …/docker.io_20.10.21-0ubuntu1~22.04.3_amd64.deb …
Распаковывается docker.io (20.10.21-0ubuntu1~22.04.3) …
Выбор ранее не выбранного пакета ubuntu-fan.
Подготовка к распаковке …/ubuntu-fan_0.12.16_all.deb …
Распаковывается ubuntu-fan (0.12.16) …
Настраивается пакет ubuntu-fan (0.12.16) …
Created symlink /etc/systemd/system/multi-user.target.wants/ubuntu-fan.service → /lib/systemd/system/ubuntu-fan.service.
Настраивается пакет runc (1.1.4-0ubuntu1~22.04.3) …
Настраивается пакет pigz (2.6-1) …
Настраивается пакет containerd (1.6.12-0ubuntu1~22.04.3) …
Created symlink /etc/systemd/system/multi-user.target.wants/containerd.service → /lib/systemd/system/containerd.service.
Настраивается пакет docker.io (20.10.21-0ubuntu1~22.04.3) …
Добавляется группа «docker» (GID 138) ...
Готово.
Created symlink /etc/systemd/system/multi-user.target.wants/docker.service → /lib/systemd/system/docker.service.
Created symlink /etc/systemd/system/sockets.target.wants/docker.socket → /lib/systemd/system/docker.socket.
Обрабатываются триггеры для man-db (2.10.2-1) …
root@Acer2010:/# sudo docker run -it -h DJC --name djc_test -v /test/folder:/otherway -v /root/test.txt:/otherway/test.txt ubuntu:22.10
Unable to find image 'ubuntu:22.10' locally
22.10: Pulling from library/ubuntu
3ad6ea492c35: Pull complete 
Digest: sha256:e322f4808315c387868a9135beeb11435b5b83130a8599fd7d0014452c34f489
Status: Downloaded newer image for ubuntu:22.10
docker: Error response from daemon: failed to create shim task: OCI runtime create failed: runc create failed: unable to start container process: error during container init: error mounting "/root/test.txt" to rootfs at "/otherway/test.txt": mount /root/test.txt:/otherway/test.txt (via /proc/self/fd/7), flags: 0x5000: not a directory: unknown: Are you trying to mount a directory onto a file (or vice-versa)? Check if the specified host path exists and is the expected type.
root@Acer2010:/# sudo docker ps -a
CONTAINER ID   IMAGE          COMMAND       CREATED         STATUS    PORTS     NAMES
b9df0390898a   ubuntu:22.10   "/bin/bash"   2 minutes ago   Created             djc_test
root@Acer2010:/# docker run --name some-mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mysql:8.0.31
Unable to find image 'mysql:8.0.31' locally
8.0.31: Pulling from library/mysql
0ed027b72ddc: Pull complete 
0296159747f1: Pull complete 
3d2f9b664bd3: Pull complete 
df6519f81c26: Pull complete 
36bb5e56d458: Pull complete 
054e8fde88d0: Pull complete 
f2b494c50c7f: Pull complete 
132bc0d471b8: Pull complete 
135ec7033a05: Pull complete 
5961f0272472: Pull complete 
75b5f7a3d3a4: Pull complete 
Digest: sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
Status: Downloaded newer image for mysql:8.0.31
c84894ab6f13b3017b13c879ae3d7d237e83ab1bbc614ce081e7935adb2b1bfd
root@Acer2010:/# docker run --name myphp -d --link some-mysql:db -p 8081:80 phpmyadmin/phpmyadmin
Unable to find image 'phpmyadmin/phpmyadmin:latest' locally
latest: Pulling from phpmyadmin/phpmyadmin
faef57eae888: Pull complete 
989a1d6c052e: Pull complete 
0705c9c2f22d: Pull complete 
621478e043ce: Pull complete 
98246dcca987: Pull complete 
bfed8c155cb6: Pull complete 
7a7c2e908867: Pull complete 
d176994b625c: Pull complete 
2d8ace6a2716: Pull complete 
c70df516383c: Pull complete 
15e1b44fe4c7: Pull complete 
65e50d44e95a: Pull complete 
77f68910bc0a: Pull complete 
605dd3a6e332: Pull complete 
99ce27188f07: Pull complete 
74d64e32c5d5: Pull complete 
ef5fc9928b9f: Pull complete 
163f3256e112: Pull complete 
Digest: sha256:67ba2550fd004399ab0b95b64021a88ea544011e566a9a1995180a3decb6410d
Status: Downloaded newer image for phpmyadmin/phpmyadmin:latest
0b8d4091aafb5b143af9c2ca8898967b97b63229cb1028230cfff59a85996586
root@Acer2010:/# sudo docker exec -it some-mysql bash
bash-4.4# mysql -u root -pmy-secret-pw
mysql: [Warning] Using a password on the command line interface can be insecure.
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 8
Server version: 8.0.31 MySQL Community Server - GPL

Copyright (c) 2000, 2022, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
4 rows in set (0.02 sec)

mysql> create database djcdb;
Query OK, 1 row affected (0.02 sec)

mysql> create database Acer2010;
Query OK, 1 row affected (0.01 sec)

mysql> use Acer2010;
mysql> use Acer2010;
Database changedble users (name varchar(20), age int, gender varchar(1), national varchar(20));
mysql> insert into users (name, age, gender, national) value ('Alex', '35', 'm', 'russian');
ERROR 1146 (42S02): Table 'Acer2010.users' doesn't exist
mysql> create table users (name varchar(15), age int, gender varchar(1), national varchar(15));
Query OK, 0 rows affected (0.04 sec)

mysql> insert into users (name, age, gender, national) value ('Alex', '35', 'm', 'russian');
Query OK, 1 row affected (0.02 sec)

mysql> show tables;
+--------------------+
| Tables_in_Acer2010 |
+--------------------+
| users              |
+--------------------+
1 row in set (0.01 sec)

mysql> 