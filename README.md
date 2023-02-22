# Docker示例项目

特色
* 多用户
* 权限与职能授权

组件
* PostgreSQL数据库
* Apache Kafka enterprise bus
* Angular前端

功能
* 项目管理
* 生产商
* 库存管理/供应链管理
* 资产管理
* 企业资源规划
  * 会计
  * 人力资源
  * 销售
  * 采购


## 安装与测试

应用程序可以使用**Docker**进行测试。转到含有docker-compose.yml文件的根目录并运行：

```
docker compose build

docker compose up -d
```
命令将构建运行应用程序本地副本所需的镜像和容器。它将运行4个容器：zookeeper实例、kafka实例、postgres数据库和应用程序二进制文件本身。可以构建并运行一个可选的容器，其中包含用于测试应用程序提供端点的swagger实例。

使用浏览器打开以下地址即可测试：

```
http://localhost
```
