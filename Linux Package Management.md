# Linux Package Management

## 1. Introduction
- Package managers handle software installation, updates, and removal.
- Different Linux distributions use different package managers.

## 2. Common Package Managers

### Debian/Ubuntu (`.deb` packages)
- **APT** (Advanced Package Tool)

  sudo apt update           # Update package list
  sudo apt upgrade          # Upgrade installed packages
  sudo apt install <pkg>    # Install a package
  sudo apt remove <pkg>     # Remove a package
  sudo apt autoremove       # Remove unused dependencies

- **dpkg (Low level Tool)**

    sudo dpkg -i <file.deb>   # Install a .deb file

    sudo dpkg -r <pkg>        # Remove a package


### RHEL/CentOS/Fedora (.rpm packages)
- **DNF** (Modern one in Fedora/RHEL)
    
    sudo dnf install <pkg>    # Install a package

    sudo dnf update           # Update all packages

    sudo dnf remove <pkg>     # Remove a package


### YUM (Older, still used in some systems)
