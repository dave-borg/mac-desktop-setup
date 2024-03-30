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
    ansible-pull -vvv -U https://github.com/dave-borg/mac-desktop-setup.git -d /Users/dborgees/mac-desktop-setup general-setup/playbook.yaml --ask-become-pass
    ```

    ### Apps
    ```bash
    ansible-pull -vvv -U https://github.com/dave-borg/mac-desktop-setup.git -d /Users/dborgees/mac-desktop-setup apps/playbook.yaml --ask-become-pass
    ```

    ### Coding
    ```bash
    ansible-pull -vvv -U https://github.com/dave-borg/mac-desktop-setup.git -d /Users/dborgees/mac-desktop-setup coding/playbook.yaml --ask-become-pass
    ```

    ### Music

    ```bash
    ansible-pull -vvv -U https://github.com/dave-borg/mac-desktop-setup.git
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
- Logic - 634148309
- Logic plugins?
- iReal pro - 409035833
- Guitar Pro
- iLok software
- UA connect
- HX Edit