# FUZZ

### 什么是FUZZ？
- 模糊测试，测试技巧
- fuzzing, fuzz testing

FUZZ -> 测试案列 -> 测试目标 -> 测试结果

需要细心与耐性！

### FUZZ使用点
- 目录扫描：使用字典
- 参数扫描：对参数的值进行FUZZ
- 枚举爆破
- 隐藏参数:优惠卷漏洞
- bypass waf
- 漏洞测试


### FUZZ工具:
1. WFUZZ : kali自带，命令:wfuzz -w 字典 URL?uid=FUZ
2. FUFF
3. Burpsuite ：Intruder

### FUZZ字典收集
- 可以网上下载,利用kali、burpsuite自带的，或制作属于自己的字典

#### 目录FUZZ，一般可以挖到如下漏洞
- 未授权访问
- 隐藏页面
- 信息泄露
- 其他问题：web-INF/web,xml
- 文件上传程序，部分服务漏洞等

#### 请求参数FUZZ
- 参数，参数的值进行FUZZ
- 一层一层FUZZ测试：目录 - 文件 - 参数 - 参数的值
