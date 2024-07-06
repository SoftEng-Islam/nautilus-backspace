<h1 align="center">
    Nautilus backspace
</h1>

<p align="center">
  <img alt="GitHub Release" src="https://img.shields.io/github/v/release/alt-gnome-team/nautilus-backspace">
  <img alt="GitHub License" src="https://img.shields.io/github/license/alt-gnome-team/nautilus-backspace">
</p>

<p align="center">
Extensions for returning back to Nautilus by pressing the combination of keys assigned via Gsettings
</p>


## installation from the repository

[![Packaging status](https://repology.org/badge/vertical-allrepos/nautilus-backspace.svg)](https://repology.org/project/nautilus-backspace/versions)

### ALT Sisyphus
```shell
su -
apt-get update
apt-get install nautilus-backspace
```


## clone the Source

```shell
git clone https://github.com/alt-gnome-team/nautilus-backspace.git
cd nautilus-backspace
```

### Dependencies

#### ALT Sisyphus
```shell
su -
apt-get update
apt-get install nautilus-python libnautilus-gir
```

#### Fedora
```shell
sudo dnf update
sudo dnf install nautilus-python
```

#### Debian/Ubuntu
```shell
sudo apt update
sudo apt install python3-nautilus gir1.2-nautilus-4.0
```

#### Arch Linux
```shell
sudo pacman -Sy python-nautilus
```


### Assembly

#### System installation
```
sudo make
sudo make schemas 
```

#### User installation
```
make
make schemas 
```


## Setup

### Change of combination
```shell
gsettings set io.github.alt-gnome-team.nautilus-backspace back '<Alt>Down'
```
### Return to the default value
```shell
gsettings reset io.github.alt-gnome-team.nautilus-backspace back
```
