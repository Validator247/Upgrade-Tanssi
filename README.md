# Upgrade-Tanssi-v0.5.1

    sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.5.1/tanssi-node && chmod +x tanssi-node && sudo systemctl restart tanssid

# Upgrade-Tanssi-v0.6.0

    sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.6.0/tanssi-node && chmod +x tanssi-node && sudo systemctl restart tanssid

# Upgrade-Tanssi-v0.6.1

    sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.6.1/tanssi-node && chmod +x tanssi-node
    sudo systemctl daemon-reload
    sudo systemctl restart tanssid
    sudo journalctl -u tanssid -f -o cat

# Upgrade-Tanssi-v0.7.0

    sudo systemctl stop tanssid && cd $HOME/tanssi-data && rm -rf tanssi-node && wget https://github.com/moondance-labs/tanssi/releases/download/v0.7.0/tanssi-node && chmod +x tanssi-node && sudo systemctl restart tanssid
    
        
Check logs: 

    sudo journalctl -u tanssid -f -o cat

Create Session Key

    curl http://127.0.0.1:9944 -H \
    "Content-Type:application/json;charset=utf-8" -d \
    '{
    "jsonrpc":"2.0",
    "id":1,
    "method":"author_rotateKeys",
    "params": []
    }'

            
