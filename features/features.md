## wallet
### core
1.hd钱包地址生成
2.发送(native token/token)
3.获取总资产(num/num*price)
#### 0.账户管理
使用eth生成的地址作为账户,密钥签名发送消息登录

#### 1.hd钱包地址生成 (client)
##### btc
bitcoinlis-js js
https://github.com/bitcoinjs/bitcoinjs-lib
##### evm
ethereumjs/ethereumjs-monorepo js
https://github.com/ethereumjs/ethereumjs-monorepo
geth go
https://github.com/ethereum/go-ethereum
##### sol
solana web3.js
https://github.com/solana-labs/solana-web3.js
api:
https://solana.com/zh/docs/rpc/http
##### tron
tronweb js
https://github.com/tronprotocol/tronweb
wallet java
https://github.com/tronprotocol/wallet-cli

#### 2.发送(native token/token)
bitcoin
https://github.com/bitpay/bitcoind-rpc


#### 3.获取总资产(num/num*price)
##### num
num-> 获取token数量并缓存至clien db
使用hd钱包发起交易 -> 本地token数量变化并更新至db
如果对账对不上则主动去拉取交易记录

##### price (hd server)
拉取cex和dex的订单簿价格做价格平均值
价格平均值用于计算总资产和选定某条线路的资产价格


