# bitcoin-insomnia

Using Insomnia to query your Bitcoin node.

## Status

Under development. Not ready for general consumption just yet.

## Implementation

This collection implements some of the functions documented in the [Bitcoin RPC API Reference](https://developer.bitcoin.org/reference/rpc/index.html).

## Environment variables

This collection uses Insomnia environment variables.  Here's what I've got:

```json
{
	"username": "<YOUR USER NAME>",
	"password": "<YOUR PASSWORD",
	"protocol": "http",
	"server": "127.0.0.1",
	"port": 8332,
	"blockhash": "000000000000000000023bc3e5419ae1a8d508f531c205e7b6493732d6948c51",
	"height": 842209,
	"nblocks": 4032,
	"txid": "c3881ad26b5319191189e8301d1ea5b6ad93bc02c39365e174e8c97b178140a7",
	"verbose": true,
	"verbosity": 2,
	"vout": 1,
	"include_mempool": true
}
```

## Progress

This collection is a work in progress.

### Key
* ✅ = presently working
* ❌ = presently broken
* 🟡 = exists but is still sketch

### Blockchain RPCs
* `getbestblockhash ✅`
* `getblock ✅`
* `getblockchaininfo ✅`
* `getblockcount ✅`
* `getblockfilter ❌`
* `getblockhash ✅`
* `getblockheader ✅`
* `getblockstats ✅`
* `getchaintips ✅`
* `getchaintxstats ✅`
* `getdifficulty ✅`
* `getmempoolancestors`
* `getmempooldescendants`
* `getmempoolentry`
* `getmempoolinfo ✅`
* `getrawmempool ✅`
* `gettxout ✅`
* `gettxoutproof`
* `gettxoutsetinfo`
* `preciousblock `
* `pruneblockchain`
* `savemempool`
* `scantxoutset`
* `verifychain`
* `verifytxoutproof`

### Control RPCs
* `getmemoryinfo ✅`
* `getrpcinfo ✅`
* `help ✅`
* `logging`
* `stop`
* `uptime ✅`

### Generating RPCs
* `generateblock`
* `generatetoaddress`
* `generatetodescriptor`

### Mining RPCs
* `getblocktemplate ✅`
* `getmininginfo ✅`
* `getnetworkhashps ✅`
* `prioritisetransaction`
* `submitblock`
* `submitheader`

### Network RPCs
* `addnode`
* `clearbanned`
* `disconnectnode`
* `getaddednodeinfo`
* `getconnectioncount ✅`
* `getnettotals ✅`
* `getnetworkinfo ✅`
* `getnodeaddresses`
* `getpeerinfo ✅`
* `listbanned ✅`
* `ping ✅`
* `setban`
* `setnetworkactive`

### Rawtransactions RPCs
* `analyzepsbt`
* `combinepsbt`
* `combinerawtransaction`
* `converttopsbt`
* `createpsbt`
* `createrawtransaction`
* `decodepsbt`
* `decoderawtransaction`
* `decodescript`
* `finalizepsbt`
* `fundrawtransaction`
* `getrawtransaction`
* `joinpsbts`
* `sendrawtransaction`
* `signrawtransactionwithkey`
* `testmempoolaccept`
* `utxoupdatepsbt`

### Util RPCs
* `createmultisig`
* `deriveaddresses`
* `estimatesmartfee`
* `getdescriptorinfo`
* `getindexinfo`
* `signmessagewithprivkey`
* `validateaddress`
* `verifymessage`

### Wallet RPCs
Note: the wallet RPCs are only available if Bitcoin Core was built with wallet support, which is the default.

* `abandontransaction`
* `abortrescan`
* `addmultisigaddress`
* `backupwallet`
* `bumpfee`
* `createwallet`
* `dumpprivkey`
* `dumpwallet`
* `encryptwallet`
* `getaddressesbylabel`
* `getaddressinfo`
* `getbalance`
* `getbalances`
* `getnewaddress`
* `getrawchangeaddress`
* `getreceivedbyaddress`
* `getreceivedbylabel`
* `gettransaction`
* `getunconfirmedbalance`
* `getwalletinfo 🟡`
* `importaddress`
* `importdescriptors`
* `importmulti`
* `importprivkey`
* `importprunedfunds`
* `importpubkey`
* `importwallet`
* `keypoolrefill`
* `listaddressgroupings`
* `listlabels`
* `listlockunspent`
* `listreceivedbyaddress`
* `listreceivedbylabel`
* `listsinceblock`
* `listtransactions 🟡`
* `listunspent`
* `listwalletdir ✅`
* `listwallets ✅`
* `loadwallet ✅`
* `lockunspent`
* `psbtbumpfee`
* `removeprunedfunds`
* `rescanblockchain`
* `send`
* `sendmany`
* `sendtoaddress`
* `sethdseed`
* `setlabel`
* `settxfee`
* `setwalletflag`
* `signmessage`
* `signrawtransactionwithwallet`
* `unloadwallet ✅`
* `upgradewallet`
* `walletcreatefundedpsbt`
* `walletlock`
* `walletpassphrase`
* `walletpassphrasechange`
* `walletprocesspsbt`
