# Install Git from Source Code 

sudo apt update
sudo apt install libz-dev libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext cmake gcc
wget https://github.com/git/git/archive/refs/tags/v2.38.1.tar.gz
tar xvfz v2.38.1.tar.gz 
cd git-2.38.1
make prefix=/usr/local all
sudo make prefix=/usr/local install

git --version

git config --global user.email "jai@demo.com"
git config --global user.name "Jai"
git config --global -l

mkdir ~/repo01 
cd ~/repo01 
ls -lrt 
git init 
ls -lrt .git 
git status 

echo "demo" > file1.txt
git status 
git add file1.txt
git status 
git commit -m "this is a sample message" file1.txt 
git status 
echo "demo" > file2.txt
git status 
git add file2.txt
git status 
git commit -m "this is a sample message" file2.txt 
git status 

echo "demo" > file3.txt
echo "demo" > file4.txt
echo "demo" > file5.txt
git status 
git add --all 
git status 
git commit -m "sample files"
git status 


echo "demo 001" >> file1.txt 
git status 
git commit -m "updated file1"  file1.txt 
git log
git diff <previous_commit_id>
git diff <commit_id_1> <commit_id_1>

sudo apt install default-jdk 
## Download and install Eclipse IDE for Java 
