<h1 align="center">EmpowerChain | Circulus Testnet</h1>
<div align="center">

 ![image](https://github.com/0xSocrates/Testnet-Rehberler/assets/108215275/f5e9add1-5b55-40d2-83dd-539cbf64c266) 

# [Twitter](https://twitter.com/empowerchain_io) | [Discord](https://discord.gg/nVTPukf2) | [Github](https://github.com/EmpowerPlastic) | [Docs](https://docs.empowerchain.io/)
 
 </div>
 
## Hello everyone, the highly anticipated reward-winning testnet of EmpowerChain has started.
## Before starting the installation, here's what you need to know:
> The Testnet consists of 3 stages:

> - Stage 1: May 31st - June 6th: Network bootstrapping phase
> - Stage 2: June 7th - June 20th: Main phase
> - Stage 3: June 21st - June 25th: Stress testing phase

> Rewards have a linear vesting period of 1 year.

> KYC will be required at the end of the Testnet.
>
> Requirements: 4 CPU cores, 16GB RAM, 500+ GB SSD.
>

## Make sure to read this [documents](https://docs.empowerchain.io/testnet/overview) to find answers to all your questions about the Testnet.
For installation-related questions and discussions, you can join the Core Node Discord and Telegram channels.

### To install using a script, enter the following command:

```
curl -sSL -o empower-install.sh https://raw.githubusercontent.com/Core-Node-Team/Testnet-EN/main/Empower%20Chain/empower-install.sh && chmod +x empower-install.sh && bash ./empower-install.sh
``` 


For those who want to do a manual installation, refer to this [guide](https://github.com/Core-Node-Team/Testnet-EN/blob/main/Empower%20Chain/Manuel-Install.md)

### After completing the installation, create a wallet
```
empowerd keys add wallet
```

### Wait for synchronization and then create a validator
```
empowerd tx staking create-validator \
  --amount 1000000umpwr \
  --from wallet \
  --commission-max-change-rate "0.01" \
  --commission-max-rate "0.2" \
  --commission-rate "0.1" \
  --min-self-delegation "1" \
  --pubkey  $(empowerd tendermint show-validator) \
  --moniker $MONIKER \
  --website "websiteniz"
  --identity keybase.io idniz \
  --details "Core Node Community" \
  --chain-id circulus-1
  --y
 ```
# Useful Links

## [Commands](https://github.com/Core-Node-Team/CosmosSDK-Node/blob/main/Ortak-Komutlar.md)
## [Node Backup](https://github.com/Core-Node-Team/CosmosSDK-Node/blob/main/Yedekleme%20ve%20Ta%C5%9F%C4%B1ma.md)
## [Port Change](https://github.com/Core-Node-Team/CosmosSDK-Node/blob/main/Port%20de%C4%9Fi%C5%9Ftirme.md)
## [Sync-Peer-FAQ](https://github.com/Core-Node-Team/Cosmos-Aglarinda-Node-Calistirmak/blob/main/Sync-Peer%20Nedir.md)

<div align="center">

# Core Node 

#  [Twitter](https://twitter.com/corenodeHQ)|[Discord](https://discord.gg/fzzUAU9k)|[Telegram](https://t.me/corenodechat)  

![1500x500](https://github.com/Core-Node-Team/Testnet-TR/assets/108215275/92b50dd4-8043-4500-b906-bc8d15b75525)

## If you have any questions, you can join our Telegram chat group and Discord server.
#

</div>
