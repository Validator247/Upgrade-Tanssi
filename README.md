# Upgrade-Tanssi-v0.5.1

    sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.5.1/tanssi-node && chmod +x tanssi-node && sudo systemctl restart tanssid

Check logs: 

    sudo journalctl -u tanssid -f -o cat
