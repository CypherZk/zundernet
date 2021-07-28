# zundernet install instruction
⚠️ backup your wallet before proceeding ⚠️
## linux users

### install dependencies

```
sudo apt install python3 -y && sudo apt install python3-pip -y && pip3 install pycryptodome && pip3 install pyside2 && pip3 install psutil
```

### download and install pirate-cli

Download the pirate-cli tool [here](https://github.com/PirateNetwork/pirate/releases/tag/v5.2.0)
Or using wget by CLI
```
wget https://github.com/PirateNetwork/pirate/archive/refs/tags/v5.2.0.tar.gz
tar -xvzf v5.2.0.tar.gz
cd pirate-v5.2.0

#here the script will exit doing nothing if already installed
./zcutil/fetch-params.sh

# -j8 = using 8 threads for the compilation - replace 8 with number of threads you want to use; -j$(nproc) for all threads available
# this step might take some time
./zcutil/build.sh -j8
```

### clone the repo

```
 cd ~ && git clone https://github.com/buidl1/zundernet.git
```

### install process

```
cd zundernet && python3 zundernet.py
```
You'll be prompted to locate both komodod & pirated paths :
![installing zundernet](https://pasteimg.com/images/2021/07/28/upload.png)

By default the komodod path is hidden and located at
```
~/.komodo/PIRATE
```
To show hidden fles and folders, in Nautilus (the default Ubuntu file manager) click on the following :
![Nautilus show hidden files and folders](https://pasteimg.com/images/2021/07/28/upload2.png)

Once both path are successfully located, you'll be prompted to either create a new wallet, or import an existing one.
In both cases, you'll be prompted to secure this wallet by a password required to log into zundernet
![zunderned install complete](https://pasteimg.com/images/2021/07/28/upload3.png)
Great ! You're now logged into your wallet and ready to start using zundernet !
Just start the blockchain (you'll need to exit TreasureChest if already running)
![zunderned install complete](https://pasteimg.com/images/2021/07/28/upload3.png)
