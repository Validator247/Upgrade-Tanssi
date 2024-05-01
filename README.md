# Upgrade-Tanssi-v0.5.1

    sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.5.1/tanssi-node && chmod +x tanssi-node && sudo systemctl restart tanssid

# Upgrade-Tanssi-v0.6.0

        sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.6.0/tanssi-node && chmod +x tanssi-node && sudo systemctl restart tanssid

# Upgrade-Tanssi-v0.6.1

        sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.6.1/tanssi-node && chmod +x tanssi-node
    sudo systemctl daemon-reload
    sudo systemctl restart tanssid
    sudo journalctl -u tanssid -f -o cat


Check logs: 

    sudo journalctl -u tanssid -f -o cat
