## NOTE 
- prepare environment for testing and learningg about linux machine 


+ **Requirements** 
- vagrant 
- oracle virtualbox 
```bash 
cd 1.introduction
vagrant init ubuntu/jammy64
# edit the cofiguration file 
vagrant up 
vagrant status 
# in order to access your machine via SSH 
vagrant ssh 


# if you uupdate the config, want to apply to you machine 
vagrant reload 
vagrant halt # to shutdown 
vagrant destroy -f  # to delete the machine 

```

## testing with your newly created machine
```bash

ip addr show # show the ip address that we have configured earlier 
tree sync_data

# install testing package
sudo apt install neofetch -y 
```
## Setup a better terminal experiences 
```bash 
sudo apt update && sudo apt upgrade -y
sudo apt install fish -y 
# to use fish terminal , just type "fish"
```
- using omz with zsh 
```bash 
sudo apt install zsh -y 
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# install plugins for better exp
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting


git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

# edit the configuration inside the zshrc files to apply the configuration for the new plugins 
nano ~/.zshrc
# Ctrol + O = write 
# Ctrl + X = exit 
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

source ~/.zshrc
```