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

# Software to install manually

- Adobe Creative Cloud
- Logic Plugins
    - Waves Central
    - [SSL Download Manager](https://solidstatelogic.com/ssl-download-manager)
    - iLok License Manager
    - Slate Digital Connect
    - Spitfire Audio
    - [VocAlign](https://www.synchroarts.com/downloads#vocalign-ultra)
    - [UA Connect](https://www.uaudio.com/volt/start)
    - [LX480 Complete](https://shop.relabdevelopment.com/dashboard/orders/2803-1753-9816)
    - [Pulsar Echorec](https://pulsar.audio/download/)
- [Guitar Pro](https://www.guitar-pro.com/my-account)


# Lab setup

To deploy to a Ubuntu server:
1. Add ssh key to target server:
    ```bash
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ssh-copy-id username@remote_host
    ```
2. Run the ansible playbook for the whole lab:
    ```bash
    cd docker-server
    ansible-playbook -i 192.168.128.142, -u borg lab-playbook.yml --ask-become-pass --ask-vault-pass
    ```
