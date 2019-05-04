# server1


### OS
Install `CentOS 6.10`

### Repository
Add `epel`, `remi` repositories.
```bash
$ rpm -iUvh http://dl.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-8.noarch.rpm
$ rpm -iUvh http://rpms.remirepo.net/enterprise/remi-release-6.rpm
```


## Utilities
7Zip
```bash
$ yum install p7zip
```

rar/unrar
```bash
$ wget https://www.rarlab.com/rar/rarlinux-x64-5.5.0.tar.gz
$ tar zxvf rarlinux-x64-5.5.0.tar.gz
$ cd rar
$ sudo cp -v rar unrar /usr/local/bin/
```


### Docker
Create a `/etc/yum.repo.d/docker.repo` as below.
```text
[docker-repo]
name=Docker Repo
baseurl=https://yum.dockerproject.org/repo/main/centos/$releasever/
enabled=1
gpgcheck=1
gpgkey=https://yum.dockerproject.org/gpg
```

Then install `docker-engine`
```bash
$ yum install docker-engine
```



## 
