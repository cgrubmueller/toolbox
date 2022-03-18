# yay installation tool

yay ist einer von vielen AUR Helper. Mit diesem Tool kann man packages aus dem AUR (Arch User Repository) herrunterladen.

#### Installation

```bash
git clone https://aur.archlinux.org/yay-git.git
cd yay
makepkg -si
```

#### Alle installieren packages upgraden

```bash
yay -Syu
```

#### Interactively search and install packages from the repos and AUR
```bash
$ yay [package_name|search_term]
```

#### Synchronize and update all packages from the repos and AUR
```bash
$ yay
```
#### Synchronize and update only AUR packages
```bash
$ yay -Sua
```

#### Install a new package from the repos and AUR
```bash
$ yay -S [package_name]
```

#### Remove an installed package and both its dependencies and configuration files
```bash
$ yay -Rns [package_name]
```

#### Search the package database for a keyword from the repos and AUR
```bash
$ yay -Ss [keyword]
```

#### Remove orphaned packages (installed as dependencies but not required by any package)
```bash
$ yay -Yc
```

#### Show statistics for installed packages and system health
```bash
$ yay -Ps
```

https://linuxcommandlibrary.com/man/yay
