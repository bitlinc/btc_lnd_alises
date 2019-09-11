# Alises for Bitcoin Core - LND - Electrum Personal Server 
# *** Only works with system user 'bitcoin' ***

# Run these commands below in terminal to copy and activate alises
# *** copy / paste everything to the right of the number and replace YOUR USERNAME ex: YOUR USERNAME -> bitcoin ***
# (1) su YOUR USERNAME GOES HERE
# (2) cd ~ 
# (3) wget https://raw.githubusercontent.com/bitlinc/btc_lnd_alises/master/README.md
# (4) mv /READ.md /home/YOUR USER NAME GOES HERE/.bash_aliases
# (5) source /home/YOUR USER NAME GOES HERE/.bashrc
# ------------------------------------------------------------------------------------------------------------------------

# Alises for Bitcoin Core - LND - Electrum Personal Server 
 ##System
alias aliases='nano /media/aliases/bitlinc_aliases' 

##Bitcoin Mainnet 
alias btcmlog='tail -f /home/bitcoin/.bitcoin/debug.log'
alias btcmpi='bitcoin-cli getpeerinfo'
alias btcmcc='bitcoin-cli getconnectioncount'
alias btcmwi='bitcoin-cli getwalletinfo'
alias btcmconf='nano /home/bitcoin/.bitcoin/bitcoin.conf'
alias btcmbi='bitcoin-cli getblockchaininfo'
alias btcmgn='bitcoin-cli getnetworkinfo'
alias btcmauto='nano /etc/systemd/system/bitcoind_mainnet.service'
alias btcports='netstat -anp | grep bitcoind'

##Bitcoin Testnet
alias btctlog='tail -f /home/bitcoin/.bitcoin/testnet3/debug.log'
alias btctpi='bitcoin-cli -testnet getpeerinfo'
alias btctcc='bitcoin-cli -testnet getconnectioncount'
alias btctwi='bitcoin-cli -testnet getwalletinfo'
alias btctconf='nano /home/bitcoin/.bitcoin/testnet3/bitcoin.conf'
alias btctbi='bitcoin-cli -testnet getblockchaininfo'
alias btctgn='bitcoin-cli -testnet getnetworkinfo'
alias btctauto='nano /etc/systemd/system/bitcoind_testnet.service'

##LND Mainnet
alias lndmconf='nano /home/bitcoin/.lnd/lnd.conf'
alias lndmain='/usr/local/bin/lnd'
alias lndmunlock='lncli unlock'
alias lndmauto='nano /etc/systemd/system/lnd_mainnet.service'
alias lndports='netstat -anp | grep lnd'

##LND Mainnet
alias lndmconf='sudo nano /home/bitcoin/.lnd/lnd.conf'
alias lndmain='/usr/local/bin/lnd'
alias lndmunlock='lncli unlock'
alias lndmauto='sudo nano /etc/systemd/system/lnd_mainnet.service'
alias lndports='sudo netstat -anp | grep lnd'

##LND Testnet
#alias lndtconf='sudo nano /home/bitcoin/.lnd/testnet/lnd.conf'
#alias lndtest='/usr/local/bin/lnd --configfile=/home/bitcoin/.lnd/testnet/lnd.conf --datadir=/home/bitcoin/.lnd/testnet/data --logdir=/home/bitcoin/.lnd/testnet/logs --listen=0.0.0.0:19735 $
#alias lndtunlock='lncli --lnddir=/home/bitcoin/.lnd/testnet --rpcserver=0.0.0.0:10010 --macaroonpath=/home/bitcoin/.lnd/testnet/data/chain/bitcoin/testnet/bitcoin.macaroon --tlscertpath=lnd$
#alias lndtcreate='lncli --lnddir=/home/bitcoin/.lnd/testnet --rpcserver=0.0.0.0:10010 --macaroonpath=/home/bitcoin/.lnd/testnet/data/chain/bitcoin/testnet/bitcoin.macaroon --tlscertpath=lnd$
#alias lndtwallet='lncli --lnddir=/home/bitcoin/.lnd/testnet --rpcserver=0.0.0.0:10010 --macaroonpath=/home/bitcoin/.lnd/testnet/data/chain/bitcoin/testnet/bitcoin.macaroon --tlscertpath=lnd'
#alias lndtconnect='lndconnect  --lnddir=/home/bitcoin/.lnd/testnet --bitcoinmacaroonpath=/home/bitcoin/.lnd/testnet/data/chain/bitcoin/testnet/bitcoin.macaroon --tlscertpath=/home/bitcoin/.lnd/
#alias lndtauto='sudo nano /etc/systemd/system/lnd_testnet.service'

##Electron Personal Server Mainnet
alias epsm='cd ~/eps_mainnet/electrum-personal-server'
alias eps='electrum-personal-server'
alias epsmlog='tail -f /home/bitcoin/EPS_mainnet/eps_mainnet_log'
alias epsmstart='/home/bitcoin/.local/bin/eps_mainnet/electrum-personal-server /home/bitcoin/EPS_mainnet/config.ini'
alias epsmconf='sudo nano /home/bitcoin/EPS_mainnet/config.ini'
alias epsmauto='sudo nano /etc/systemd/system/eps_mainnet.service'

##Electron Personal Server Testnet
alias epst='cd ~/eps_testnet/electrum-personal-server'
alias epstlog='tail -f /home/bitcoin/EPS_testnet/eps_testnet_log'
alias epststart='/home/bitcoin/.local/bin/eps_testnet/electrum-personal-server /home/bitcoin/EPS_testnet/config.ini'
alias epstconf='sudo nano /home/bitcoin/EPS_testnet/config.ini'
alias epstauto='sudo nano /etc/systemd/system/eps_testnet.service'

##Electrum Wallet Mainnet
alias emauto='sudo nano /etc/systemd/system/electrum_wallet_mainnet.service'
alias electrummstart='su pi -c "electrum --oneserver --server=192.168.2.4:50003:s"'

##Electrum Wallet Testnet
alias etauto='sudo nano /etc/systemd/system/electrum_wallet_testnet.service'
alias electrumtstart='su pi -c "electrum --testnet --oneserver --server=192.168.2.4:50004:s"'
