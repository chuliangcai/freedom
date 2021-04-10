### 前言
公司进行安全整改，要求代码里面不能直接把密钥存放在配置文件里。解决办法就是使用vault存储，然后使用spring-cloud-vault-config和spring的配置文件进行整合，最终的效果就是，密钥以`key-value`的形式存储在vault中，代码里只需要在properties文件里使用占位符获取即可，比如
```properties
spring.datasource.password=${mysql.password}
```
使用起来超级方便，今天就和我一起探索vault的世界吧！

### 使用docker安装vault server和vault UI
参考：https://learn.hashicorp.com/tutorials/vault/getting-started-ui?in=vault/getting-started
参考
因为vault知识偏向运维，这次不做深入研究

### 附录
* vault启动web ui https://learn.hashicorp.com/tutorials/vault/getting-started-ui?in=vault/getting-started
* docker vault 