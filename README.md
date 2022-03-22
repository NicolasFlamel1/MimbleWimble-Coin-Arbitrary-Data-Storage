# Storing the Mimblewimble whitepaper on the MimbleWimble Coin floonet blockchain

### Description
Arbitrary data can be stored in a kernel's lock height if the data interpreted as a number is less than or equal to the current block height. By doing this I was able to store the [Mimblewimble whitepaper by Tom Elvis Jedusor](https://scalingbitcoin.org/papers/mimblewimble.txt) on the MimbleWimble Coin floonet blockchain within 5183 kernels. At approximately 2.5 bytes of arbitrary data allowed per kernel using this method at current block heights, it isn't efficient nor economical to store arbitrary data in this way.

### Running
Run the following command while passing in a node's address as a command line argument to the program to get the Mimblewimble whitepaper from that node. This example uses the node address `https://mwc713.floonet.mwc.mw`. This program will default to using the node address `http://localhost:13413` if no node address is provided. This program can take awhile to finish running when using it with an external node, so it's recommended to run this against a local node.
```
python3 main.py https://mwc713.floonet.mwc.mw
```
