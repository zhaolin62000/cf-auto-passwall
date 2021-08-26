## 自动替换 PassWall 里面的 WS 节点地址 为 CF 优选的IP


用途：用于自动筛选 CF IP，并自动替换优选 IP 为 PassWall 的节点地址

感谢YouTube频道：波仔分享

本脚本源于 GitHub：Lbingyi 以及 Paniy

本教程视频演示地址：https://youtu.be/WzRHi9f9QKg

使用说明：加在 openwrt 上系统 计划任务里 添加定时运行，如 0 4 * * 2,4,6 bash /root/cf-auto-passwall.sh > /dev/null

0 4 * * 2,4,6 的意思是在每周二、周四、周六的凌晨4点会自动运行一次。/root/cf-auto-passwall.sh 是你脚本的绝对地址

> 时程表的格式如下:
> 
> f1 f2 f3 f4 f5 program
> 
> 其中 f1 是表示分钟，f2 表示小时，f3 表示一个月份中的第几日，f4 表示月份，f5 表示一个星期中的第几天。program 表示要执行的程式。
>
> 0 03 * * * 表示每天的凌晨三点

## 注意事项

1、请在脚本中修改你期望优选 IP 的带宽大小（默认50M）

2、请更改 421 行 的 xxxxxxxxxx 字符串，为你自己 PassWall 的节点值

3、不会请看博客 https://www.v2rayssr.com/cf-auto-passwall.html

