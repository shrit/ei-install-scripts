# Script Tests

Tests use VirtualBox and Vagrant to ensure a consistent validation of the installation scripts.

## Requirements

You can use homebrew to install most of the test requirements

- VirtualBox
    ```
    brew install --cask virtualbox
    ```
- VirtualBox Extension Pack
    ```
    brew install --cask virtualbox-extension-pack
    ```
- Vagrant
    ```
    brew install --cask vagrant
    ```
- Vagrant Manager (optional)
    ```
    brew install --cask vagrant-manager
    ```
- Vagrant Guest Additions plugin (optional)
    ```
    vagrant plugin install vagrant-vbguest
    ```

## Getting Started

1. Switch to the directory for the box you want to test:
    - For Windows 10:
        ```
        cd boxes\windows-10
        ```
2. Start the vagrant box and wait for the command to finish (may take several minutes)
    ```
    vagrant up
    ```
3. Log into the box via ssh (use the default vagrant password)
    ```
    vagrant ssh
    ```
4. Switch to the vagrant directory
    - On Windows:
        ```
        cd C:\vagrant
        ```
6. Run the installation script
    - On Windows:
        ```
        .\install-windows.ps1
        ```