-----------------------------------------------------

### Install Python 3.8.7
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
-----------------------------------------------------
### Install NodeJS-NPM
```shell
# Step 1 – Prerequisite 
```
