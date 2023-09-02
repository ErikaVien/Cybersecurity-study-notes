## 渗透测试 Penetration Testing
- 目标系统授权的情况下，采取可控的入侵手法，达到保护重要资产的目的地
- 软件测试，如: app, 网页，machine like ATM

渗透操作系统：Kali Linux, Parrot Securiy Os, Blackbox, BlackArch, Win10-kali, Ninjutsu

Kali所属组织：Offensive security, Exploit-Database, Vulnhub
### 安全三要素：CIA
  - 保密性 confidentiality : 机密
  - 完整性 integrity ： 数据受否被篡改
  - 可用性 availability ：业务能正常运行

### 渗透测试对象：
1. 网络硬件设备: 个人电脑，服务器，WAF, Firewall, IDS, Physical security, IoT
2. 主机操作系统: Windows, Linux, UNIX, MacOs, DNS server, etc
3. 应用系统: 软件，web系统，Framework，Javascript, Docker, 中间件，QQ, etc
4. 数据库系统 : Oracle, Mysql, DB2, SYBASE, PostgreSQL, Foxpro, etc

_硬件-系统操作-应用-数据库_

### 渗透测试意义：
1. 发现漏洞
2. 了解安全状态
3. 重视风险
4. 提升防护水平

### 渗透流程：
1. **确定目标：**
- 范围 ：什么可以做不可以做的，对域名，设备之类
- 规则(限制条件)：内网外网，社会工程学，
- 需求
2. **信息收集：** 域名信息，IP，开放的端口，文件，目录结构，软件版本，网站框构，WAF之类
3. **漏洞扫描**
- vulnerability vs bugs : vulnerability 安全性的，可导致恶意代码或信息泄露而bugs是功能缺陷
- 漏洞数据库: 参看CVE www://cve.mitre.org/,CNVD,CNNVD
- 扫描工具 : 扫描漏洞存在，自动化的工具，如Appscan,Nessue,AWVS
- 漏洞分类：可参考CNNVD
4. **漏洞利用:** 攻击，防御绕过，维持访问（后渗透攻击）
5. **清除痕迹/形成报告**
  - 发现什么漏洞
  - 危害性
  - 怎么发现的
  - 如何复现
  - 原因分析
  - 修补建议

