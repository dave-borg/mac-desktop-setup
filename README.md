# Mac Desktop Setup

## Prerequisites 

1. Install Brew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Install Ansible

```bash
brew install ansible
```

3. Run installers

    ### General setup
    ```bash
    ansible-pull -U https://github.com/dave-borg/mac-desktop-setup.git -d /Users/dborgees/mac-desktop-setup general-setup/playbook.yaml --ask-become-pass
    ```

    ### Apps
    ```bash
    ansible-pull -U https://github.com/dave-borg/mac-desktop-setup.git -d /Users/dborgees/mac-desktop-setup apps/playbook.yaml --ask-become-pass
    ```

    ### Coding
    ```bash
    ansible-pull -U https://github.com/dave-borg/mac-desktop-setup.git
    ```

    ### Music

    ```bash
    ansible-pull -U https://github.com/dave-borg/mac-desktop-setup.git
    ```

## General setup and preferences
- Update OSX
```bash
sudo softwareupdate -ia --restart
```

- bash alias
- dock size and magnification
- Ranch VPN

## Apps
- Adobe Creative Cloud
- Bitwarden
- Dropbox
- MS Remote Desktop
- MS Edge



### Homebrew
- warp
- bbedit
- mas
- nmap
- ffmpeg
- aichat
- btop
- ca-certificates
- curl
- flac
- gh
- remind
- htop
- sshpass
- mas
- wget
- wireshark
- nmap
- numpy
- yt-dlp


## Coding
- Xcode
- vs code
- Postman
- VirtualBox

### MAS
- Xcode


### Homebrew
- ansible
- git
- vscode
- docker
- docker-completion
- docker-compose
- sqlite
- sqlite-utils
- maven
- mysql
- node
- openjdk

## Music
- Logic
- Logic plugins?
- iReal pro
- Guitar Pro
- iLok software
- UA connect
- HX Edit


## Homebrew Packages

