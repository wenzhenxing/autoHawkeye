# autoHawkeye
鹰眼自动化运维监控系统（<a href="https://github.com/autohawkeye/autoHawkeye/wiki/%E8%87%AA%E5%8A%A8%E5%8C%96%E7%9B%91%E6%8E%A7%E7%B3%BB%E7%BB%9F%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8EV1.0">系统截图及使用见WIKI</a>）
<img src="https://raw.githubusercontent.com/autohawkeye/autoHawkeye/master/image/QQ%E6%88%AA%E5%9B%BE20180912175305.png"/>
<img src="https://github.com/autohawkeye/autoHawkeye/blob/master/image/QQ%E6%88%AA%E5%9B%BE20180912175820.png?raw=true"/>
<img src="https://github.com/autohawkeye/autoHawkeye/blob/master/image/QQ%E6%88%AA%E5%9B%BE20180912180538.png?raw=true"/>
<img src="https://github.com/autohawkeye/autoHawkeye/blob/master/image/QQ%E6%88%AA%E5%9B%BE20180919225058.png?raw=true"/>

目的：开发一款简单好用，好上手的监控系统，成为运维人员的好帮手。

服务端开发语言： Java

客户端（Agent）：Python

运行环境：jdk1.8及以上、Tomcat7.0及以上,如果大家的TOMCAT有兼容的问题，也可以使用我提供的TOMCAT 版本

客户端适配：因为是在centos 环境开发，只能确定支持centos6.5及以上版本，暂不清楚是否支持其它的系统

实现功能如下：

1. 应用运行状态及实现应用的健康检查，应用于HTTP的服务，通过检查健康检查地址来确定应用是否能够提供服务。

2. TCP 端口监控，主要是针对外提供非HTTP服务的应用，只要有端口就可以监控它的存活性。

3. redis 中间件的监控，内存使用率，KEY数量，连通性，命中率等指标进行监控。

4. mysql 数据库监控，监控连接数，QPS /TPS ，缓存池使用率，增删改查提交回滚分量，流量接收发送，慢查询日志数量等，并提供丰富的图表展示。

5. 主机信息统计，通过启动客户端Agent 自动统计主机相关的信息，磁盘大小，内存大小，CPU核数，系统版本，Agent版本等。

6. 磁盘监控，总量，使用量，使用率，超过设定的使用率则提醒报警， 提供图表展示。

7. 磁盘IO，监控磁盘的繁忙程度，详细的数据，磁盘使用率，超过设定的使用率则提醒报警，提供图表展示。

8. 内存监控，使用内存超过设定值则提醒报警，提供图表展示。

9. CPU 负载， 通过收集1分钟，5分钟，15分钟的CPU负载数据，单核负载超过设定值则报警，提供图表展示。

10. 网络流量监控，通过收集主机流量收发数据，展示进出网络流量，设定报警值，提供图表展示。

11. 用户管理，添加可登录本系统人员，以及设置可接收报警邮件的人员相关信息，短信报警暂不提供

12. 邮件服务器设置，亲测可支持QQ邮箱，163邮箱，公司邮箱也是可以支持的。

13. 报警邮件模版可定制

14. 记录历史报警邮件

以上功能还有待完善及改进，希望大家多提出意见或建议，技术交流QQ群：818087362
