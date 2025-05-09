## Connect two machines to have shared folder

### 1. Host Side

#### create folder
- ``mkdir share``
- ``chmod 755 share``

#### add exports
- ``sudo nano /etc/exports``

#### edit file, add line
add (for whole subnet, but better to give conciete IP access)
``/home/username/shared 192.168.1.0/24(rw,sync,no_subtree_check)``

#### enabled and restart
- ``sudo exportfs -a``
- ``sudo systemctl restart nfs-kernel-server``

#### check if configured
- ``showmount -e localhost``

### 2. Client Side

#### create folder
- ``mkdir ~/nfs-share``

#### mount folder to exported hosts folder 
- ``sudo mount -t nfs 192.168.1.36:/home/username/shared ~/nfs-share``

NOTE: after reboot client configuration will be reset and it is require to mount again
