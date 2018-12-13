
[点击查看中文](README_CN.md)

## docker images 
You should update the last version from https://hub.docker.com/r/boscore/bos/tags/

## Clone project

```
git clone https://github.com/boscore/bos-testnet.git
cd fullnode
```

## Setup a fullnode in 5 seconds using the shell

```
./run.sh
```

## Setup a fullnode manually in 1 minute

The first step, create the desired directory:

```
mkdir -p /data/eos/nodeos-data-volume/nodeos-data-bostest/data
```

The second step is to prepare the configuration file:

```
cp -r config /data/eos/nodeos-data-volume/nodeos-data-bostest
```

The third step, join the network:

```
docker-compose -f docker-compose-bostest-init.yaml up -d
```

## Stop/Restart syncing

To stop:

```
docker-compose -f docker-compose-bostest.yaml down
```

To restart:

```
docker-compose -f docker-compose-bostest.yaml down
docker-compose -f docker-compose-bostest.yaml up -d
```

## Chain info

```

"chain_id": "33cc2426f1b258ef8c798c34c0360b31732ea27a2d7e35a65797850a86d1ba85"

```

## P2P LIST

```
p2p-peer-address = 120.197.130.116:9000
p2p-peer-address = 13.230.195.142:9866
p2p-peer-address = 120.197.130.117:9000
p2p-peer-address = 120.197.130.117:9001
p2p-peer-address = 120.197.130.117:9002
p2p-peer-address = 120.197.130.117:9003
p2p-peer-address = 45.79.145.205:9000
p2p-peer-address = 47.91.244.124:443
p2p-peer-address = 8.208.9.182:443
p2p-peer-address = 47.254.82.241:443
p2p-peer-address = 47.254.134.167:443
p2p-peer-address = 149.129.133.66:443
```


## HTTP API LIST

API nodes:
```

```

API nodes support get actions ( filter-on=* ):
```

```

## Faucet

Creating accounts on bostest is pretty simple:

#### Free Account
Create account using: http://13.230.195.142/create_account?new_account_name

Example:
```
curl http://13.230.195.142/create_account\?111111111ooo
```


#### Get Free tokens
Get free token with: http://13.230.195.142/get_token?your_account_name.   

## telegram monitor 
https://t.me/bosteststatus 
