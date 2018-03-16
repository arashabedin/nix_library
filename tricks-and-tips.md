# 1.Getting the latest version of nodejs and npm

## Using Ubuntu
curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
sudo apt-get install -y nodejs


## Using Debian, as root
curl -sL https://deb.nodesource.com/setup_9.x | bash -
apt-get install -y nodejs

# Show a commit tree like in GUI git clients
git log --graph --decorate --oneline --all (there are other options for this)

*To make this permanent add this as an alias to your .gitconfig file located in your home folder*
For example adding this will show you the commit history whenever you type "git tree"

[Aliases]
tree = log --graph --decorate --oneline --all


