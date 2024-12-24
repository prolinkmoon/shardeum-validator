# Shardeum Validator
### Step by step to running Shardeum Validator

#### Official shardeum link:
* [Testnet Portal](https://shardeum.org/incentivized-testnet)
* [Twitter / X](https://x.com/shardeum)
* [Official Docs](https://docs.shardeum.org/docs)

### Minimum Hardware and/or other Requirements

* 250 GB SSD storage
* Quad core CPU less than 10 years old if self hosting
* Dual core CPU works if hosted with newer Xeons / EPYC
* 16 GB of ram, 4+ GB of virtual memory recommended
* Hosting: 8 GB RAM + 8 GB Virtual Memory

* 10 SHM token, is a minimun stake into your Validator. you can req Faucet SHM Token on [Discord](https://discord.gg/6BNAkxFz)

## Let's touch your VPS Terminal
```bash
sudo apt update && apt upgrade -y
```
```bash
sudo apt-get install curl git-all -y
```
```bash
sudo apt install docker.io
```
```bash
docker --version
```
*check your docker version. ensure Docker version 20.10.12 or higher

## Download and Install Validator

```bash
curl -O https://raw.githubusercontent.com/shardeum/shardeum-validator/refs/heads/itn4/install.sh && chmod +x install.sh && ./install.sh
```

#### The terminal will ask questions about your setup settings.

Give permission to collect validator data for bug reporting:
```
By running this installer, you agree to allow the Shardeum team to collect this data. (y/n)?:
```
Enter y to setup the web based dashboard (Y):
```
Do you want to run the web based Dashboard? (y/n):
```
Set a password for dashboard access ( Don't forget to save your password for access dasboard ):
```
Set the password to access the Dashboard:
```
Add a custom session port for the web based dashboard or hit enter for port 8080 ( Recomended change it, eg: 8081):
```
Enter the port (1025-65536) to access the web based Dashboard (default 8080):
```
Add a custom external IP address or use an automatically detected IP address ( enter to skip ):
```
If you wish to set an explicit external IP, enter an IPv4 address (default=auto):
```
Add a custom internal IP address or use an automatically detected IP address ( enter to skip ):
```
If you wish to set an explicit internal IP, enter an IPv4 address (default=auto):
```
Set the first p2p port (default 9001, Recomended change it, eg: 9002):
```
To run a validator on the Sphinx Atomium network, you will need to open two ports in your firewall.
This allows p2p communication between nodes.
Enter the first port (1025-65536) for p2p communication (default 9001):
```
Set the second p2p port (default 10001, Recomended change it, eg: 10002):
```
Enter the second port (1025-65536) for p2p communication (default 10001):
```
Add a custom path or install to root, ( enter ):
```
What base directory should the node use (defaults to ~/.shardeum):
```

Wait download and installation done perfectly ..


### Open validator GUI

Go to your web browser and go to:
```
https://<your-VPS-IP>:<Port-web-based-Dashboard>   eg; https://168.120.125.48:8081
```
* Input your Password that you have set up previously
* Connect your Metamask Wallet
* req faucet on discord
* Start your node
* Stake 10+ SHM token
* Done! Happy testing 😊





