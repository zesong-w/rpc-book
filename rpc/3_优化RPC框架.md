# 3、优化RPC框架

在刚才实现的RPC框架中，其实隐藏者许多问题需要去解决：

- 服务的注册和发现需要手动完成
- 序列化采用的是JDK的默认方式，效率较低
- 网络模型采用的是BIO，而且是短连接，效率很差

接下来，我们就一一解决这些问题，对框架进行升级
