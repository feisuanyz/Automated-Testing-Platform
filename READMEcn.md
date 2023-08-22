全自动测试平台
-----------------------------------
语言：[中文](https://github.com/feisuanyz/Automated-Testing-Platform/blob/main/READMEcn.md) | [English](https://github.com/feisuanyz/Automated-Testing-Platform/blob/main/README.md)

最新版本客户端：[Windows和Linux版本](https://main.feisuanyz.com:8080/atp/feisuanyz-local-client.zip)

安装环境配置要求：

| 类别       | 要求                        |
|----------|---------------------------|
| 操作系统     | Windows 7（64位） 及以上或者Linux |
| CPU      | 推荐 i5 以上                  |
| 运行内存     | 推荐 16 G 以上                |
| 软件安装磁盘容量 | 至少1 GB 容量以上               |

历史版本客户端及安装配置说明，请查阅[《ATP Installation Resource》](https://github.com/feisuanyz/Automated-Testing-Platform/tree/main/.%20ATP%20Installation%20Resource)。

===============================================

全自动测试平台，覆盖整个软件测试的生命周期管理，包含测试用例管理、测试计划管理、接口测试、性能测试等功能，并且完全兼容JMeter，可以一键关联和同步Java全自动开发工具的项目和项目中所有的接口信息，通过高度自动化的测试来赋能团队进行高质量的软件交付和整体测试效率的提升。

### 客户端部署说明

全自动测试平台支持使用本地客户端，即支持用户在本地服务器上使用全自动测试平台。在全自动测试平台下载本地客户端并启动成功后，即可通过本地服务器访问全自动测试平台。同时本地客户端还支持多端登录，多账户时无需单独配置，直接在多个浏览器页面同时登录即可。

#### 1. 前提条件

用户需在Linux或Windows系统中安装Java环境。

#### 2. 操作步骤

a）进入解压后的文件夹，双击startup.bat，启动本地客户端。

![image](https://github.com/feisuanyz/testplatform/assets/79617492/0e20dd13-fa2d-4208-9899-c7a20f539724)

b）若出现如图所示程序，即说明本地客户端启动成功。

![image](https://github.com/feisuanyz/testplatform/assets/79617492/0ba777a1-89b6-4ea5-99d1-7a59892984ac)

c）在浏览器地址栏输入本地服务器地址加上端口号，回车进入登录页面。

说明：c1）此处输入的端口号需确保未被占用，默认为8080；若需修改端口号，可在application.yml配置文件中修改端口，application.yml配置文件内容如下所示，端口号可自行设置；c2）本地客户端运行性能测试需要填写host地址，host为部署本地客户端的服务地址。

```
server:
  port: 8080

atp:
  platform:
    # 部署机器地址，如172.16.101.35，不要配置localhost、127.0.0.1
    host: 172.16.101.35
```

![image](https://github.com/feisuanyz/testplatform/assets/79617492/0f44d375-0870-43f0-a62c-886c412ceaad)

d）输入正确的账号和密码，登录成功即可正常访问全自动测试平台。

说明：d1）通过本地客户端访问全自动测试平台的账号密码，与通过飞算云智官网访问全自动测试平台的账号密码一致；d2）也可在浏览器中新建页面，输入地址后用不同账号登录本地客户端，此时可以多个账号同时登录并互不干扰。

![image](https://github.com/feisuanyz/testplatform/assets/79617492/4b669f82-2ab3-48c4-b812-4bc426b771e9)
