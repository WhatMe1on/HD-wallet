## wallet
### core
1.hd钱包地址生成
2.发送(native token/token)
3.获取总资产(num/num*price)
#### 1.hd钱包地址生成
##### btc
####
##### evm

##### sol
##### tron

#### 2.发送(native token/token)

#### 3.获取总资产(num/num*price)
##### num
num-> 获取token数量并缓存至clien db
使用hd钱包发起交易 -> 本地token数量变化并更新至db
如果对账对不上则主动去拉取交易记录
hd服务端扫链时 发现有其他钱包转向hd钱包 -> 通知客户端更新交易数据
 
##### price
拉取cex和dex的订单簿价格做价格平均值
价格平均值用于计算总资产和选定某条线路的资产价格


