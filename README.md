### 更新
2019年11月6日
   - [x] 修复了上次更新存在的问题，神马牛鬼蛇神的报告都能导出了

2019年10月30日

   - [x] 修复了上次更新存在的问题，神马牛鬼蛇神的报告都能导出了
   
   - [x] 任务中带有特殊符号，无法在Windows下创建文件时，统一更名为“多任务输出+微秒级时间戳”
   
   - [x] 把1.8改成了2.0

2019年10月17日

   - [x] 修复了多任务输出的报告导出失败
   
   - [x] 修复了编辑过的报告导出失败

2018年4月25日
   - [x] 着手写，并正式开源

### 工具介绍
绿盟远程安全评估系统漏洞数据导出工具，只支持RSAS6.0以上版本。

工具涉及：读取目录下的文件、ZIP文件读取、正则表达式、Excel表格写入、文件读写、PyQt5、TKinter(舍弃)

### 功能

- [x] 自定义漏洞等级
- [x] 自定义导出数据
- [x] 自定义Excel模板
- [x] 支持导出的数据：主机名、IP地址、端口、协议、服务、漏洞名称、风险等级、整改建议、漏洞描述、漏洞CVE编号、扫描起始时间、扫描结束时间、漏洞扫描月份
- [x] 导出不同端口的同一个漏洞，也就是一个端口对应一个漏洞，保证导出漏洞的完整性。
- [x] 导出端口和导出网站为单独的功能，导出网站的功能是采用正则去匹配http、www这两个服务。

### 须知
- [x] 当一个漏洞存在两个或者两个以上CVE编号，则只取第一个CVE漏洞编号。
- [x] 当一个漏洞不存在CVE编号时，则替换为 漏洞暂无CVE编号 。
- [x] 当一个漏洞整改建议为空时（个别低危漏洞），导出留空。

### 下载
下载链接是Windows版本的，如果需要在其他平台使用，可下载源码自己打包。

https://github.com/autoing/RSAS-Data-Export/releases

### 使用方法

导出的原始报告必须勾选主机报表才行，程序是直接读取zip的，不能解压，把原始报告放到一个文件夹内，路径选择对应的文件夹就可以了。

![](https://autoing.github.io/do/images/tool/rsas_1.8.gif)
