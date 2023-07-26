```
docker pull ubuntu

docker run -it --volume=C:\Users\IcingTomato\Documents\M5Stack\STM32MP1:/mnt -d ubuntu /bin/bash

docker attach xxx
```

useradd -g root espresso -s /bin/bash -p espresso -M

sed -i 's@//.*archive.ubuntu.com@//mirrors.ustc.edu.cn@g' /etc/apt/sources.list && apt update

sudo vmhgfs-fuse .host:/STM32MP1 /mnt  -o allow_other

apt-get -y install locales file bsdmainutils libgmp-dev libmpc-dev libssl-dev lz4 pylint gawk wget git-core diffstat unzip texinfo gcc-multilib build-essential chrpath socat cpio python3 python3-pip python3-pexpect xz-utils debianutils iputils-ping python3-git python3-jinja2 libegl1-mesa libsdl1.2-dev xterm nano repo git

git config --global http.proxy http://192.168.2.24:7890 && git config --global https.proxy http://192.168.2.24:7890

sed -i '/en_US.UTF-8/s/^# //g' /etc/locale.gen && locale-gen

mkdir -p /mnt/Distribution-Package && cd /mnt/Distribution-Package

repo init -u https://github.com/STMicroelectronics/oe-manifest.git -b refs/tags/openstlinux-6.1-yocto-mickledore-mp1-v23.06.21

```
rm -rf /usr/bin/python && ln -s /usr/bin/python3 /usr/bin/python

git config --global user.email "icing@m5stack.com" && git config --global user.name "IcingTomato"

cp /mnt/Distribution-Package/.repo/repo/repo /usr/bin/repo

rm -rf /usr/bin/python && ln -s /usr/bin/python2 /usr/bin/python

repo init -u https://github.com/STMicroelectronics/oe-manifest.git -b refs/tags/openstlinux-6.1-yocto-mickledore-mp1-v23.06.21

https://github.com/Seeed-Studio/stm32mp1-manifest

repo init -u https://github.com/Seeed-Studio/stm32mp1-manifest.git

```

repo sync -j8

repo sync -j8 --fail-fast

```
git clone https://git.yoctoproject.org/poky openembedded-core && cd openembedded-core && git checkout -t origin/mickledore
```

DISTRO=openstlinux-weston MACHINE=stm32mp13-disco source layers/meta-st/scripts/envsetup.sh

export CONNECTIVITY_CHECK_URIS="http://www.baidu.com"

bitbake st-image-weston





sudo apt-get install open-vm-tools -y

vmware-hgfsclient

sudo vmhgfs-fuse .host:/STM32MP135 ~/mnt -o allow_other






