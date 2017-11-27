.PHONY: build cluster test

default: build

build:
	go build -o bin/swarm    github.com/w3eleft/go-ethereum/cmd/swarm
	go build -o bin/geth     github.com/w3eleft/go-ethereum/cmd/geth
	go build -o bin/bootnode github.com/w3eleft/go-ethereum/cmd/bootnode

cluster: build
	scripts/boot-cluster.sh

test:
	go test -v github.com/w3eleft/go-ethereum/swarm/...
