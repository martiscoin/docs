---
icon: file
label: Node
---
# Node API

You can use this API to interact with a wallet, check the balance, or build a transaction.
It contains all the necessary methods for developing an application or integrate Martiscoin into your system.

### Methods
---

#### `getinfo`

Gets general information about the full node.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getinfo
```

#### `getblockcount`

Gets the current consensus tip height.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getblockcount
```

#### `getblockheader`

Gets the block header of the block identified by the hash.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getblockheader {hash}
```

#### `validateaddress`

Returns information about a bech32 or base58 bitcoin address.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 validateaddress {address}
```

#### `getblock`

Returns the block in hex, given a block hash.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getblock {blockHash}
```

#### `getnetworkinfo`

Returns an object containing various state info regarding P2P networking.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getnetworkinfo
```

#### `getblockchaininfo`

Returns an object containing various state info regarding blockchain processing.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getblockchaininfo
```

#### `addnode`

Adds a node to the connection manager..{command}:add,remove,onetry

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 addnode {ip} {command}
```

#### `getpeerinfo`

Gets peer information from the connection manager.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getpeerinfo
```