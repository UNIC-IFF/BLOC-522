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

Here is a list of the APIs generated on the succesfull deployment of the Besu Private Network=
```
JSON-RPC HTTP service endpoint : http://<HOST_IP>:8545
JSON-RPC WebSocket service endpoint : ws://<HOST_IP>:8546
Web block explorer address : http://<HOST_IP>:25000/
Prometheus address : http://<HOST_IP>:9090/graph
Grafana address : http://<HOST_IP>:3000/d/XE4V0WGZz/besu-overview?orgId=1&refresh=10s&from=now-30m&to=now&var-system=All
```