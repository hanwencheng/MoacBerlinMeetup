## Berlin MOAC Meetup

1. generate genesis blockchain, confirm network id
./moac --datadir ./chainData init ../genesis.json 


2. start vnode, mining
./moac --datadir ./chainData --verbosity 4 --networkid 8666


vnode Opened: /Users/hanwencheng/Documents/moac/vnode/chainData/moac.ipc
./moac attach /Users/hanwencheng/Documents/moac/vnode/chainData/moac.ipc


3. Create Account
personal.newAccount()

4. start miner
miner.start()

5. run moac rpc node
./moac --datadir ./chainData --rpc --rpccorsdomain "http://wallet.moac.io"


NOTICE: before send the transaction, unlock first.
personal.unlockAccount(mc.coinbase, 'password', 0)
