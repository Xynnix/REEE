------------------------------------------------------
# Linux | Debian 9/10

## Python3.8
### Install Python 3.8.7 [Non-Root]
```shell
# Step 1 – Prerequisite
sudo apt-get install build-essential checkinstall -y
sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev \
    libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev libffi-dev zlib1g-dev -y

#Step 2 – Download Python 3.8
cd /opt
sudo wget https://www.python.org/ftp/python/3.8.7/Python-3.8.7.tgz
sudo tar xzf Python-3.8.7.tgz

# Step 3 – Compile Python Source
cd Python-3.8.7
sudo ./configure --enable-optimizations
sudo make altinstall

# Step 4 – Check Python Version
python3.8 -V

# Step 5 – Remove Python
cd /opt
sudo rm -f Python-3.8.7.tgz
```
### Install Python 3.8.7 [Root/Admin]
```shell
# Step 1 – Prerequisite
apt-get install build-essential checkinstall -y
apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev \
    libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev libffi-dev zlib1g-dev -y

#Step 2 – Download Python 3.8
cd /opt
wget https://www.python.org/ftp/python/3.8.7/Python-3.8.7.tgz
tar xzf Python-3.8.7.tgz

# Step 3 – Compile Python Source
cd Python-3.8.7
./configure --enable-optimizations
make altinstall

# Step 4 – Check Python Version
python3.8 -V

# Step 5 – Remove Python
cd /opt
rm -f Python-3.8.7.tgz
```
-----------------------------------------------------
## NodeJS 14.x
### Install NodeJS-NPM [Non-Root]
```shell
# Step 1 – Prerequisite
sudo apt update && sudo apt-get install curl software-properties-common

# Step 2 – Download NodeJS 14.x
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -

# Step 3 – Install NodeJS-NPM via APT
sudo apt install nodejs

# Step 4 – Check NodeJS Version
node -v
```
### Install NodeJS-NPM [Root/Admin]
```shell
# Step 1 – Prerequisite
apt update && sudo apt-get install curl software-properties-common

# Step 2 – Download NodeJS 14.x
curl -sL https://deb.nodesource.com/setup_14.x | -E bash -

# Step 3 – Install NodeJS-NPM via APT
apt install nodejs

# Step 4 – Check NodeJS Version
node -v
```
