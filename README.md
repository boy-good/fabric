# fabric
java sdk demo for fabric

本地Window 在 VirtualBox虚拟机中安装 Ubuntu 16.04 的环境
搭建运行Fabric 1.4版本

使用 bootstrap.sh pull docker images & fabric-samples
使用 byfn.sh 启动 first-network 网络（一个 orderer,两个 org，每个org有两个 peer）

使用 startFabric.sh 启用fabcar chaincode的网络，并在远程用fabric-sdk-java调用

## BYFN network running success.
![node running](https://github.com/boy-good/fabric/blob/master/images/BYFN.png)

## chaincode invoke success and return transaction ID.
![chaincode invoke](https://github.com/boy-good/fabric/blob/master/images/Invoke.png)

## query chaincode fabcar by key:CAR1
![chaincode query](https://github.com/boy-good/fabric/blob/master/images/Query.png)
