# btc_lnd_alises
# Set for user 'bitcoin'
# run this command in terminal in /home/Bitcoin to download and active the aliases
# (1) wget https://raw.githubusercontent.com/bitlinc/btc_lnd_alises/master/README.md
# (2) mv /home/bitcoin/README.md /home/bitcoin/.bash_aliases
# (3) source /home/bitcoin/.bashrc
# -------------------------------------------------------------------------------------

# Alises for Bitcoin Core - LND - Electrum Personal Server 
 6 ##System
 7 alias my_alias='nano /home/bitcoin/.bash_aliases'
 8 alias reload_bash='source /home/bitcoin/.bashrc'
 9
10 ##Bitcoin Mainnet 
11 alias btcmlog='tail -f /home/bitcoin/.bitcoin/debug.log'
12 alias btcmpi='bitcoin-cli getpeerinfo'
13 alias btcmcc='bitcoin-cli getconnectioncount'
14 alias btcmwi='bitcoin-cli getwalletinfo'
15 alias btcmconf='nano /home/bitcoin/.bitcoin/bitcoin.conf'
16 alias btcmbi='bitcoin-cli getblockchaininfo'
17 alias btcmgn='bitcoin-cli getnetworkinfo'
18 alias btcmauto='nano /etc/systemd/system/bitcoind_mainnet.service'
19 alias btcports='netstat -anp | grep bitcoind'
20
21 ##Bitcoin Testnet
22 alias btctlog='tail -f /home/bitcoin/.bitcoin/testnet3/debug.log'
23 alias btctpi='bitcoin-cli -testnet getpeerinfo'
24 alias btctcc='bitcoin-cli -testnet getconnectioncount'
25 alias btctwi='bitcoin-cli -testnet getwalletinfo'
26 alias btctconf='nano /home/bitcoin/.bitcoin/testnet3/bitcoin.conf'
27 alias btctbi='bitcoin-cli -testnet getblockchaininfo'
28 alias btctgn='bitcoin-cli -testnet getnetworkinfo'
29 alias btctauto='nano /etc/systemd/system/bitcoind_testnet.service'
30
31 ##LND Mainnet
32 alias lndmconf='nano /home/bitcoin/.lnd/lnd.conf'
33 alias lndmain='/usr/local/bin/lnd'
34 alias lndmunlock='lncli unlock'
35 alias lndmauto='nano /etc/systemd/system/lnd_mainnet.service'
36 alias lndports='netstat -anp | grep lnd'

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
alias epsmlog='tail -f /home/bitcoin/EPS_mainnet/eps_mainnet_log'
alias epsmstart='/home/bitcoin/.local/bin/eps_mainnet/electrum-personal-server /home/bitcoin/EPS_mainnet/config.ini'
alias epsmconf='sudo nano /home/bitcoin/EPS_mainnet/config.ini'
alias epsmauto='sudo nano /etc/systemd/system/eps_mainnet.service'
##Electron Personal Server Testnet
alias epstlog='tail -f /home/bitcoin/EPS_testnet/eps_testnet_log'
alias epststart='/home/bitcoin/.local/bin/eps_testnet/electrum-personal-server /home/bitcoin/EPS_testnet/config.ini'
alias epstconf='sudo nano /home/bitcoin/EPS_testnet/config.ini'
alias epstauto='sudo nano /etc/systemd/system/eps_testnet.service'

##Electrum Wallet Mainnet
alias emauto='sudo nano /etc/systemd/system/electrum_wallet_mainnet.service'
alias electrum_mainnet_start='electrum --oneserver --server=192.168.2.4:50003:s'

##Electrum Wallet Testnet
alias etauto='sudo nano /etc/systemd/system/electrum_wallet_testnet.service'
alias electrum_testnet_start='electrum --testnet --oneserver --server=192.168.2.4:50004:s'

##Scripts
alias my_scripts='cd ~/.local/bin/cryptoOS_scripts'
alias verify_software='~/.local/bin/cryptoOS_scripts/gpg_verify.sh'
alias stop_all='~/.local/bin/cryptoOS_scripts/stop.sh'
alias auto_start='cd /etc/systemd/system'
