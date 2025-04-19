# 透明代理升级案例

The Web3 社区透明代理升级课堂演示实战代码

### 安装依赖
```
forge install foundry-rs/forge-std --no-commit
forge install OpenZeppelin/openzeppelin-contracts --no-commit
forge install OpenZeppelin/openzeppelin-contracts-upgradeable --no-commit
```

### 项目构建
```
forge build
```

### 启动 anvil 本地节点
```
anvil
```

### 部署升级测试

```
# 环境变量配置
export PRIVATE_KEY=0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80

# 部署第一版本的合约
forge script ./script/TreasureManagerScript.s.sol:TreasureManagerScript --rpc-url 127.0.0.1:8545 --private-key 0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80 --broadcast
```
