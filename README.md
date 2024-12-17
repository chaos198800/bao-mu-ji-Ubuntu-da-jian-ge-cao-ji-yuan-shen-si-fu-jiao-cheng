# 保姆级Ubuntu搭建割草机（原神私服）教程

欢迎来到详尽的Ubuntu系统下原神私服——“割草机”的搭建指南。本教程专为希望在Linux环境下自建《原神》私有服务器的玩家设计。我们将逐步引导您完成整个过程，从环境配置到服务器启动，确保即便是新手也能顺利架设自己的游戏空间。

## **准备工作**

- **系统要求**：首选Ubuntu 20.04 LTS，以避免因OpenSSL版本兼容性导致的问题。
- **必备工具**：SSH客户端（如Terminal），FTP软件（例如WinSCP）。
- **环境配置**：
  - 安装Java JDK 17。
  - 部署MongoDB数据库（推荐使用稳定的版本，如4.0系列，避免最新版可能的兼容性问题）。

## **关键步骤概览**

1. **安装基础软件**：
   - 使用apt-get命令更新及升级系统。
   - 安装JDK 17和MongoDB，注意数据库的正确配置以允许远程访问。

2. **下载必要组件**：
   - 获取Grasscutter服务端jar文件。
   - 拉取Resources资源库，这是游戏数据的核心。
   - 下载必要的插件，如gc-opencommand-plugin，并配置。

3. **配置环境**：
   - 更新配置文件`config.json`，包括数据库连接、服务端口、资源路径等。
   - 创建并设置正确的文件结构，如`/home/grasscutter`内包含`GC-Resources`、`plugins`等目录。

4. **服务端启动**：
   - 使用Java命令运行Grasscutter jar文件，首次运行会自动生成必需的配置文件和目录。

5. **代理设置**：
   - 为客户端访问设置代理，确保网络通讯顺畅。

6. **客户端调整**：
   - 根据所搭建的服务器版本，下载相应客户端并应用特定补丁。
   - 修改客户端设置，指向您的私服地址。

7. **注意事项**：
   - 解决IPv6可能导致的连接问题，关闭不必要的IPv6服务。
   - 确保服务器防火墙规则允许所需的TCP/UDP端口访问。

通过遵循上述步骤，您就能成功搭建属于自己的《原神》私服，享受私人定制的游戏体验。每一步的细节操作，包括命令示例和可能遇到的常见问题，在原始文章中有详细解释，务必仔细阅读每一步指导，确保搭建过程无障碍。祝您搭建顺利，游戏愉快！

## 下载链接

[保姆级Ubuntu搭建割草机原神私服教程](https://pan.quark.cn/s/3391a91c7aa4)