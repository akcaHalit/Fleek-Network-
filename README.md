! We are going to be on Phase{4} 
Then on Phase{5} will be mainnet

<h1 align="center">Fleek Network</h1>

> [Phase0](https://blog.fleek.network/post/fleek-network-testnet-phase0/)

<h1 align="center"> Hardware</h1>


```console
# Ubuntu 22.04 
4 CPU 8 RAM
```

#

> Add USER
```console
# change the darthlyrex
adduser darthlyrex
usermod -aG sudo darthlyrex
su darthlyrex
cd /home/darthlyrex
```

<h1 align="center"> SETUP </h1>

```console
# Updates
sudo apt update && sudo apt upgrade -y

sudo fallocate -l 10240M /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile

# We install rust and libraries and choose 1 in the options:
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
rustup update
```

```console
# The steps we are installing with the script may take a very long time, it depends on your server performance.
curl https://get.fleek.network | bash
# Say yes to Yes/No questions.

# Once the installation is complete, we will be given the Node Public Key and Consensus Public Key. Save it.
```

> Meanwhile, get tokens from [here](https://faucet.testnet.fleek.network/) and open a fleek wallet.
> 
```console
# Start the server
sudo systemctl start lightning.service
sudo systemctl stop lightning.service
sudo systemctl restart lightning.service
```

> Enter the information from where you minted and complete the transaction.

> Control Command: `curl -sS https://get.fleek.network/healthcheck | bash`

![image](https://github.com/ruesandora/Fleek/assets/101149671/c042eef0-f50e-42b3-88e0-2845bf7201f0)





