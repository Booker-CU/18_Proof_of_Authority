# 18_Proof_of_Authority

ZChain Blockchain

In order to get node1 up and mining, use the following command-line:

./geth --datadir node1  --rpc --mine --minerthreads 1 

#this command will start mining for the first node
#make sure to copy the enode address for next step
#when it asks for a password, please enter the password we have provided*
--rpc flag:enables the http server
--mine: starts mining process
--minerthreads: specifies how many parallel threads to use


To get node2 up and mining please use code below in a new terminal window:
#be sure to navigate to the designated zchain folder on your machine

./geth --datadir node2 --port 30304 --mine --minerthreads 1 --bootnodes "enode://<your new enode address goes here>"
--bootnodes: instructs geth nodes to use our own bootnode  
  
zchain
ChainId = 777

*Password for zchain network, and to start mining each node: zblock

Connecting to MyCryptoWallet
In order to connect to the zchain blockchain on MyCryptoWallet
-open MyCryptoWallet and change the network to the zchain network

-use connect to wallet using keystore file and navigate to the node1/keystore folder and select the UTC file

#this should unlock the wallet and you should see the public address for node1

#to send a transaction put the address you would like to send Ether to and select the amount to send

#you should get a transaction hash

#additional images attached
