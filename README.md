# tft
Terraform Test - not a WC3 Addon :)

# Install WSL
Source: https://docs.microsoft.com/en-us/windows/wsl/install-manual
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

# Install Docker Desktop (for Windows)
Source: https://docs.docker.com/desktop/windows/install/

# Install Remote - WSL in VSC
Source: https://code.visualstudio.com/docs/remote/wsl-tutorial

# RSA key generate
Source: https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04-de

```bash
ssh-keygen
```

# Clone git repo
```bash
git clone git@github.com:tp199314/tft.git
git config --global user.name "tp199314"
git config --global user.mail "fake@example.de"
```

# Install Terraform on Ubuntu (WSL)
Source: https://learn.hashicorp.com/tutorials/terraform/install-cli

```bash
sudo apt-get update; sudo apt-get upgrade -y; sudo apt-get dist-upgrade -y; sudo apt-get autoremove -y; sudo apt-get autoclean -y; sudo apt-get install git

sudo apt-get update && sudo apt-get install -y gnupg software-properties-common curl
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt-get install terraform

terraform -install-autocomplete
```