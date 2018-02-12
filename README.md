# CropCoin
Shell script to install a [Beetle Masternode](https://beetlecoin.io) on a Linux server running Ubuntu 16.04. Use it on your own risk.  

***
## Installation:  

wget -q https://raw.githubusercontent.com/zoldur/Beetle/master/beetle.sh  
chmod +x ./beetle.sh  
./beetle.sh
***

## Desktop wallet setup  

After the MN is up and running, you need to configure the desktop wallet accordingly. Here are the steps:  
1. Open the Beetle Desktop Wallet.  
2. Go to RECEIVE and create a New Address: **MN1**  
3. Send **50000** BEET to **MN1**.  
4. Wait for 15 confirmations.  
5. Go to **Tools -> "Debug console"**  
6. Type the following command: **masternode outputs**  
7. Go to **Masternodes** tab  
8. Click **Create** and fill the details:  
* Alias: **MN1**  
* Address: **VPS_IP:PORT**  
* Privkey: **Masternode Private Key**  
* TxHash: **First value from Step 6**  
* Output index:  **Second value from Step 6**  
* Reward address: leave blank  
* Reward %: leave blank  
9. Click **OK** to add the masternode  
10. Click **Start All**  

***

## Usage:  

For security reasons **Beetle** is installed under **beetlecoin** user, hence you need to **su - beetlecoin** before chcking:    

```
su - beetle
beetled masternode status
beetled getinfo
```  

***

  
Any donation is highly appreciated  

**BEET**: Bd63fusv7fXKz7zynxh7kRmVafJ19ujo8V  
**BTC**: 1BzeQ12m4zYaQKqysGNVbQv1taN7qgS8gY  
**ETH**: 0x39d10fe57611c564abc255ffd7e984dc97e9bd6d  
