# eureka-server
eureka 注册中心 

# 1. 高可用
* 若一台服务器模拟  需要修改/ect/hosts 添加配置
  ``127.0.0.1 server1 server2``
  那个注册地址及为server1:port/eureka,server2:port/eureka
* 若多台 只需要修改注册中心ip即可
_遗留问题：部署在阿里云linux服务器上时,自动读取的ip为内网地址,若本地注册服务将无法调用阿里云上服务,可能真实部署都在一个网络环境中_
# 2. linux 后台执行jar命令
  ``java -jar eureka-server1-0.0.1-SNAPSHOT.jar  >eureka-server-log.file 2>&1 &``
