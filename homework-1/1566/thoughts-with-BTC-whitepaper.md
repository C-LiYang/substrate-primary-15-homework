# 观后感
中本聪为解决中心化金融机构的信用问题，提出了使用哈希，数字签名，共识算法，p
2p广播技术构造的一个去中心化的电子货币系统。

## 哈希算法和共识
哈希算法是一个单向函数，通过输入可以很简单的计算输出，但是如果要反向计算，需要暴力穷举，并且可以控制穷举难度，给POW机制提供了理论依据。通过使用merkle hash，也使得区块的交易具备了不可篡改的特性。

## 数字签名
数字签名是p2p交易最重要的一部分，他解决了中介的信用问题，可以构造无需中介参与的交易。比特币的数字签名使用了ECDSA椭圆曲线签名算法。当拥有私钥的人对交易进行签名后，任何人都可以根据公钥和签名来验证交易是否合法。

## 广播与共识
通过对区块充分的广播，共识一致的节点将维护一份相同的账本，节点之间采取最长链的共识，但某一个时刻，网络中可能会存在多条分叉出来的链，但是因为最长链原则，最终数据会保持一致，并且链越长，被篡改的可能性就越小，矿工会为了追求利益，而共同维护网络的稳定性。