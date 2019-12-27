### Enable DeltaRPM and Fastest Mirror Plugins
Add these lines at the end of this file /etc/dnf/dnf.conf
```
fastestmirror=true
deltarpm=true
```

### Update and Upgrade Your System
```
sudo dnf upgrade
```

### Install Multimedia Plugins
```
sudo dnf install gstreamer1-plugins-base gstreamer1-plugins-good gstreamer1-plugins-ugly gstreamer1-plugins-bad-free gstreamer1-plugins-bad-free gstreamer1-plugins-bad-freeworld gstreamer1-plugins-bad-free-extras ffmpeg
```

### Fedy Installation
```
sudo dnf copr enable kwizart/fedy
sudo dnf install fedy -y
```

### Some Applications
```
sudo dnf install wine vlc icedtea-web java-openjdk p7zip p7zip-plugins unrar
```

### Enable RPM Fusion
```
sudo rpm -Uvh http://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
sudo rpm -Uvh http://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
```

### Snap Installation
```
sudo dnf install kernel-debug-modules
sudo dnf install snapd
sudo ln -s /var/lib/snapd/snap /snap
sudo snap install snap-store
```
