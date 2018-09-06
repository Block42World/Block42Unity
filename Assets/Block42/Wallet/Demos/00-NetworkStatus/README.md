![Block42](http://assets.block42.world/images/icons/block42_logo_200.png)

# Block42 Unity Wallet Demo 0 - Network Status
The pre-first demo shows the chain network status, such as block number, miner, etc.

## Demo Scene
Open [NetworkStatusDemo.unity](NetworkStatusDemo.unity) scene, a [NetworkStatusDemo.cs](NetworkStatusDemo.cs) is attached at DemoScript.

Run play, the info will be retrived and printed out:
![Screenshot](/Documents/Demo-00-NetworkStatusDemo/01_screenshot.png)

## Scripts Overview
In [NetworkStatusDemo.cs](NetworkStatusDemo.cs), it uses EthXxxxRequest from Nethereum library to interact with the chosen blockchain:

**EthBlockNumberUnityRequest**:
Gets the total block number in the chaiin.

**EthGasPriceUnityRequest**:
Gets the current gas price in the chain.

**EthGetBlockWithTransactionsByNumberUnityRequest**:
Gets the block info given a block number in the chain.

Notes that EthXxxxRequest is a coroutine and has to run using `StartCoroutine()`. More use-cases and explanations for different EthXxxxRequest will be cover in next demos.