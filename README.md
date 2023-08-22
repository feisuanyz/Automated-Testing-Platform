Automated Testing Platform（ATP）
-----------------------------------
Language: [English](https://github.com/feisuanyz/Automated-Testing-Platform/blob/main/README.md) | [中文](https://github.com/feisuanyz/Automated-Testing-Platform/blob/main/READMEcn.md)

Client Download：[For Windows & Linux](https://main.feisuanyz.com:8080/atp/feisuanyz-local-client.zip)

Installation Environment：

| Category       | Requirement         |
|----------|----------------|
| Operating System    | Windows 7 and above 64-bit or Linux|
| CPU      | i5 or above(Recommended)   |
| RAM     |  16 GB or above(Recommended)    |
| Disk | 1 GB or above    |

For previous client versions and installation instructions, please refer to [ATP Installation Resource](https://github.com/feisuanyz/Automated-Testing-Platform/tree/main/.%20ATP%20Installation%20Resource).

===============================================

Automated Testing Platform（a.k.a ATP） covers the entire software testing lifecycle management, including test case management, test plan management, interface testing, performance testing, and more. It is fully compatible with JMeter and can easily associate and synchronize projects and interface information from Java Automated Development Tool with just a single click. Enabling highly automated testing empowers teams to deliver high-quality software and improve overall testing efficiency.

### Client Deployment Instructions

Automated Testing Platform provides local client, allowing users to use the platform on their local servers. After downloading and successfully launching local client, users can access ATP through their local servers. ATP local client also supports multiple logins, where users can login in simultaneously on multiple browser pages without separate configurations.

#### 1. Prerequisites

Users should have Java environment installed on their Linux or Windows systems.

#### 2. Steps

a) Enter the extracted folder and double-click on startup.bat to launch local client.

![image](https://github.com/feisuanyz/testplatform/assets/79617492/0e20dd13-fa2d-4208-9899-c7a20f539724)

b) If the program appears as shown in the image, it means local client has been successfully launched.

![image](https://github.com/feisuanyz/testplatform/assets/79617492/0ba777a1-89b6-4ea5-99d1-7a59892984ac)

c) Enter the local server address followed by port number in Browser and press Enter to access login page.

Note: c1) The input port number here should be ensured to be unoccupied, defaulting to 8080. If you need to modify port number, it can be done in the application.yml file, whose content is shown below, and port number can be set accordingly. 

c2) To run performance tests with ATP local client, a host address indicating where ATP local client is deployed must be filled in.

```
server:
  port: 8080

atp:
  platform:
    # Deployment machine address, such as 172.16.101.35, do not configure localhost or 127.0.0.1
    host: 172.16.101.35
```

![image](https://github.com/feisuanyz/testplatform/assets/79617492/0f44d375-0870-43f0-a62c-886c412ceaad)

d）Enter the correct account and password to log in and access Automated Testing Platform.

Note: d1) Account and password for accessing Automated Testing Platform via local client is the same as those via feisuan official website.

d2) Alternatively, you can open a new browser page and log in to local client with different accounts. In this case, multiple accounts can be logged in simultaneously without interference.

![image](https://github.com/feisuanyz/testplatform/assets/79617492/4b669f82-2ab3-48c4-b812-4bc426b771e9)
