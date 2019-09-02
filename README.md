# btc_lnd_alises
# Set for user 'bitcoin'
# run this command in terminal in /home/Bitcoin to download and active the aliases
# wget https://raw.githubusercontent.com/bitlinc/btc_lnd_alises/master/README.md
# mv /home/bitcoin/README.md /home/bitcoin/.bash_aliases
##System
alias my_alias='sudo nano /home/bitcoin/.bash_aliases'
alias reload_bash='source /home/bitcoin/.bashrc'

##Bitcoin Mainnet 
alias btcmlog='~/.local/bin/cryptoOS_scripts/bitcoin_scripts/mainnet/./btcmlog'
alias btcmpi='bitcoin-cli getpeerinfo'
alias btcmcc='bitcoin-cli getconnectioncount'
alias btcmwi='bitcoin-cli getwalletinfo'
alias btcmconf='sudo nano /home/bitcoin/.bitcoin/bitcoin.conf'
alias btcmbi='bitcoin-cli getblockchaininfo'
alias btcmgn='bitcoin-cli getnetworkinfo'
alias btcmauto='sudo nano /etc/systemd/system/bitcoind_mainnet.service'
alias btcports='sudo netstat -anp | grep bitcoind'

##Bitcoin Testnet
alias btctlog='~/.local/bin/cryptoOS_scripts/bitcoin_scripts/testnet/./btctlog'
alias btctpi='bitcoin-cli -testnet getpeerinfo'
alias btctcc='bitcoin-cli -testnet getconnectioncount'
alias btctwi='bitcoin-cli -testnet getwalletinfo'
alias btctconf='sudo nano /home/bitcoin/.bitcoin/testnet3/bitcoin.conf'
alias btctbi='bitcoin-cli -testnet getblockchaininfo'
alias btctgn='bitcoin-cli -testnet getnetworkinfo'
alias btctauto='sudo nano /etc/systemd/system/bitcoind_testnet.service'

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
