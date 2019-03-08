# fabric
java sdk demo for fabric

本地Window 在 VirtualBox虚拟机中安装 Ubuntu 16.04 的环境（Git、Docker）
搭建运行Fabric 1.4版本

使用 bootstrap.sh pull docker images & fabric-samples

1、使用 byfn.sh 启动 first-network 网络（一个 orderer,两个 org，每个org有两个 peer）

2、使用 startFabric.sh 启用fabcar chaincode的网络，并在远程用fabric-sdk-java调用

## BYFN network running success.
![node running](https://github.com/boy-good/fabric/blob/master/images/BYFN.png)

## chaincode invoke success and return transaction ID.
![chaincode invoke](https://github.com/boy-good/fabric/blob/master/images/Invoke.png)

## query chaincode fabcar by key:CAR1
![chaincode query](https://github.com/boy-good/fabric/blob/master/images/Query.png)

## 使用 cli 查询账本

docker exec cli peer chaincode query -C mychannel -n fabcar -c '{"Args":["queryCar","CAR1"]}'
![CLI query](https://github.com/boy-good/fabric/blob/master/images/CLIQuery.png)

# HUAWEI CLOUD 华为云区块链服务BCS

购买区块链服务 填写相关配置即快速部署节点（私链或者联盟链）

使用华为云提供的API，下载对应的配置，就可以与链交互，而不用直接使用Fabric SDK

基本版区块链服务虽然免费，但是需要购买云服务器，文件存储等

