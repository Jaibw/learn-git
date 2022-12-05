# Install Git from Source Code 

sudo apt update
sudo apt install libz-dev libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext cmake gcc
wget https://github.com/git/git/archive/refs/tags/v2.38.1.tar.gz
tar xvfz v2.38.1.tar.gz 
cd git-2.38.1
make prefix=/usr/local all
sudo make prefix=/usr/local install
git --version

