# Linux Package Management

## 1. Introduction
- Package managers handle software installation, updates, and removal.
- Different Linux distributions use different package managers.

## 2. Common Package Managers in Linux

### Debian/Ubuntu (`.deb` packages)
- **APT** (Advanced Package Tool)
>
    sudo apt update           # Update package list

    sudo apt upgrade          # Upgrade installed packages
    
    sudo apt install <pkg_name> # Install a Package
    
    sudo apt remove <pkg_name # Remove Package
    
    sudo apt autoremove       # Remove unused dependencies

- **dpkg (Low level Tool)**
>
    sudo dpkg -i <file.deb>   # Install a .deb file

    sudo dpkg -r <pkg_name>        # Remove a package


### RHEL/CentOS/Fedora (.rpm packages)
- **DNF** (Modern one in Fedora/RHEL)
>
    sudo dnf install <pkg_name>    # Install a package
    sudo dnf update           # Update all packages
    sudo dnf remove <pkg_name>     # Remove a package


### YUM (Older, still used in some systems)
    yum install <package_name>  # Install a Package
    yum remove <package_name> # Remove packages and also any dependencies
    yum update # Updates all the installed packages
    yum info <package_name> # Shows info about a package and its dependencies
    yum search <keyword> # Searches for a package in the repositories based on a keyword.
    
### Arch Linux
    sudo pacman -S <package_name>  # Installing the package
    sudo pacman -Syu # Updating the existing packages
    sudo pacman -R <package_name> # Removes the existing package by the package name
