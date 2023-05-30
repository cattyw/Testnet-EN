<h1 align="center">EmpowerChain | Circulus Testnet</h1>
<div align="center">
image

Twitter | Discord | Github | Docs
 </div>
Hello everyone, the highly anticipated reward-winning testnet of EmpowerChain has started.
Before starting the installation, here's what you need to know:
The Testnet consists of 3 stages:

Stage 1: May 31st - June 6th: Network bootstrapping phase
Stage 2: June 7th - June 20th: Main phase
Stage 3: June 21st - June 25th: Stress testing phase
Rewards have a linear vesting period of 1 year.

KYC will be required at the end of the Testnet.

Requirements: 4 CPU cores, 16GB RAM, 500+ GB SSD.

Make sure to read this document to find answers to all your questions about the Testnet.
For installation-related questions and discussions, you can join the Core Node Discord and Telegram channels.
To install using a script, enter the following command:
bash
Copy code
curl -sSL -o empower-installation.sh https://raw.githubusercontent.com/Core-Node-Team/Testnet-TR/main/Empower%20Chain/empower-installation.sh && chmod +x empower-installation.sh && bash ./empower-installation.sh
For those who want to do a manual installation, refer to this guide.
After completing the installation, create a wallet
csharp
Copy code
empowerd keys add wallet
Wait for synchronization and then create a validator
lua
Copy code
empowerd tx staking create-validator \
  --amount 1000000umpwr \
  --from wallet \
  --commission-max-change-rate "0.01" \
  --commission-max-rate "0.2" \
  --commission-rate "0.1" \
  --min-self-delegation "1" \
  --pubkey  $(empowerd tendermint show-validator) \
  --moniker $MONIKER \
  --website "yourwebsite" \
  --identity keybase.io username \
  --details "Core Node Community" \
  --chain-id circulus-1 \
  --yes
Useful Links
Commands
Backing up and Moving the Node
Changing Ports
Sync Peer FAQ
<div align="center">
Core Node
Twitter | Discord | Telegram
1500x500

If you have any questions, you can join our Telegram chat group and Discord server.
</div>
