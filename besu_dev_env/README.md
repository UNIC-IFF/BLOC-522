# BLOC 522: Smart Contract Programming
This is a repository including the nessesary scripts and tutorials for: 
1) Deploy a private besu network
2) Build a docker image with ganache and truffle suite

For #1 you need to clone this repository and CD in submodule [quorum-dev-quickstart @ 49bf4a3](https://github.com/ConsenSys/quorum-dev-quickstart/tree/49bf4a309747977be00684139e5655747e22381e)

First, make sure you have docker and docker-compose installed as well as Nodejs (version >= 12). Installation guides are included in that directory.

Then, you run the command 
```
npx quorum-dev-quickstart
```

After the succesfull geenration of the needed files you move into the newly created repository and you run 
```
./run.sh
```

More details are given within the submodule's directory.

Here is a list of the APIs generated on the succesfull deployment of the Besu Private Network
```
JSON-RPC HTTP service endpoint : http://<HOST_IP>:8545
JSON-RPC WebSocket service endpoint : ws://<HOST_IP>:8546
Web block explorer address : http://<HOST_IP>:25000/
Prometheus address : http://<HOST_IP>:9090/graph
Grafana address : http://<HOST_IP>:3000/d/XE4V0WGZz/besu-overview?orgId=1&refresh=10s&from=now-30m&to=now&var-system=All
```

Currently, a deployment of a Besu private network is deployed on the Contabo VM with IP: **173.212.239.47**

In the following picture it is depicted the integration of the network within Metamask

<p align="center"><img src="https://github.com/UNIC-IFF/BLOC-522/blob/main/figures/bloc522-Metamask%20add%20besu%20network.jpg"/></p>

The following accounts are funded with ETH tokens derived from the pre-funded accounts of the besu client

```
•	0xC03E57b6acE9Dd62C84A095E11E494E3C8FD4D42 ( Panayiotis 15K ETH)
•	0xe8B098Dbf5210B24594868D593A9517A0a884CF8 (Klitos 100K ETH)
•	0x603a576235b75FdEcb49962a9516FdeDe09B7af5 (Evgenia 15k ETH)
•	0x8D50374B56150d56022e08251230b119E7B61D00 (Marios 50k ETH)
```

