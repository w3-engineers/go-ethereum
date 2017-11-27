This repository is custom fork of https://github.com/w3eleft/go-ethereum

## Change Log

Stop empty block mining reward
consensus/ethash/consensus.go

Create a different network than main ethereum network

params/config.go

core/genesis.go

mobile/params.go

cmd/utils/flags.go

params/bootnodes.go

cmd/geth/chaincmd.go

cmd/geth/main.go

cmd/geth/usage.go

## Update Geth

    sudo rm /usr/bin/geth
    sudo cp build/bin/geth /usr/bin/geth
    
## Start

    geth --leftnet
    
Or with rpc and custom directory    
    
    geth --leftnet --nodiscover --datadir="privchain" --rpc --rpcport 8545 --rpcaddr 0.0.0.0 --rpccorsdomain "*" --rpcapi "eth,net,personal,web3"