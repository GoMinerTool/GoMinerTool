<div id="top"></div>

<!-- PROJECT LOGO -->
<div align="center">

<img src="https://raw.githubusercontent.com/MinerProxyBTC/GoMinerTool/main/image/slogo.png#gh-light-mode-only" alt="Logo" width="200" height="200">

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
<!-- ![Github stars](https://img.shields.io/github/stars/MinerProxyBTC/GoMinerTool.svg) -->

# GoMinerTool
  <p align="center">
    <h2>抽水恒定千分之3，无递增，纯转发不抽水</h2>
    <h3>Web操作界面，简单易用，小白也可轻松上手，支持ETH/ETC/BTC/LTC/CFX/RVN/ERG/XMR/等多个币种抽水，欢迎对比、实测</h3>
    <img src="./image/jt1.png" alt="Logo">
    <a href="https://kdocs.cn/l/slPG1q488Trc"></a>
    Telegram交流群：<a href="https://t.me/+Qam442PoHcs0YmIx">https://t.me/+Qam442PoHcs0YmIx</a>
  </p>
</div>


Linux一件安装脚本：

```
bash <(curl -s -L https://raw.githubusercontent.com/MinerProxyBTC/GoMinerTool/main/linux-install.sh)
```
完整复制命令运行；默认帐号admin，密码admin123；设置好以后切记更改密码！


# 软件预览

<p id="preview"></p>
<img src="./image/jt1.png" alt="Logo">
<img src="./image/tinified/jt3.png" alt="Logo">
<img src="./image/tinified/jt2.png" alt="Logo">
<!-- <img src="./image/tinified/t5.png" alt="Logo"> -->
<img src="./image/tinified/t6.png" alt="Logo">
<img src="./image/tinified/t7.png" alt="Logo">
<img src="./image/tinified/t8.png" alt="Logo">
<img src="./image/tinified/t9.png" alt="Logo">


# 简单教程

<ol>
<li>
    <a href="#preview">软件预览</a>
</li>
  <li>
    <a href="#install">安装软件</a>
    <ul>
        <li>
            <a href="#linux">Linux</a>
            <ul>
                <li>
                    <a href="#linux">安装</a>
                </li>
                <li>
                    <a href="#linux">更新</a>
                </li>
                <li>
                    <a href="#linux">卸载</a>
                </li>
                <li>
                    <a href="#linux">停止</a>
                </li>
                <li>
                    <a href="#linux">启动</a>
                </li>
                <li>
                    <a href="#linux">重启</a>
                </li>
                <li>
                    <a href="#linux">开机启动</a>
                </li>
                <li>
                    <a href="#linux">设置最大连接数</a>
                </li>
                <li>
                    <a href="#linux">查看程序运行时日志</a>
                </li>
            </ul>
        </li>
        <li>
            <a href="#windows">Windows</a>
        </li>
    </ul>
</li>

  <li>
    <a href="#about">常见问题</a>
    <ul>
        <li>
            <a href="#q15">内存相关</a>
        </li>
        <li>
            <a href="#q0">进程守护</a>
        </li>
        <li>
            <a href="#q1">默认账号密码</a>
        </li>
        <li>
            <a href="#q1">算力呈现波浪状</a>
        </li>
        <li>
            <a href="#q2">负载均衡</a>
        </li>
        <li>
            <a href="#q3">安装时提示 curl: command not found</a>
        </li>
        <li>
            <a href="#q4">修改端口启动</a>
        </li>
        <li>
            <a href="#q5">修改密码</a>
        </li>
        <li>
            <a href="#q6">启动时提示 dial tcp connection refused</a>
        </li>
        <li>
            <a href="#q7">关闭/删除端口</a>
        </li>
        <li>
            <a href="#q8">安装时提示：安装killall失败！！！！请手动安装psmisc后再执行安装程序。</a>
        </li>
        <li>
            <a href="#q9">WEB访问长时间卡在LOADING界面。</a>
        </li>
        <li>
            <a href="#q11">IP黑名单</a>
        </li>
        <li>
            <a href="#q12">ETH芯片机和芯动A11系列相关问题</a>
        </li>
        <li>
            <a href="#q13">本地算力修改</a>
        </li>
        <li>
            <a href="#q14">迁移</a>
        </li>
        <li>
            <a href="#q10">开发费用及算力损失问题</a>
        </li>
    </ul>
</li>
<li>
    <a href="#uplog">更新日志</a>
</li>

<li><a href="#about">免责声明</a></li>
<li><a href="#about">联系我们</a></li>
</ol>

</p>


<!-- GETTING STARTED -->
<p id="install"></p>


<p id="linux"></p>

# Linux


root用户直接执行以下命令, 根据提示选择对应功能即可。
```
bash <(curl -s -L https://raw.githubusercontent.com/MinerProxyBTC/GoMinerTool/main/linux-install.sh)
```
### 安装完成之后, 请立即修改登录账号、密码以及启动端口，防止被爆破。

<img src="./image/t12.png" alt="Logo">

支持的Linux

* Ubuntu 64 18.04+
* Centos 64 7+

<p id="windows"></p>

# Windows
下载完后直接启动即可，程序自带进程守护

<a href="https://github.com/MinerProxyBTC/GoMinerTool/tree/main/Windows-64">下载地址</a>


<p id="question"></p>
<p id="about"></p>

___

<span id="q0"></span>
> # 常见问题
>>## 进程守护
>>>程序自带了进程守护, 不要！不要！不要使用supervisor或相关工具维护进程，否则会导致进程重复开启。
>><span id="q1"></span>
>>## 算力呈现波浪状
>>><img src="./image/t10.png" alt="Logo"><br>
>>>
>>>如果出现上图中的情况, 说明您开启了多个相同端口的GoMinerTool, 关闭多余的进程即可。
>>>
>>>如果您进行了镜像拷贝，也会出现以上问题，先执行脚本停止程序的运行，然后删除掉/root/GoMinerTool/license文件, 再执行启动即可
>><span id="q2"></span>
>>## 负载均衡
>>>等待更新
>><span id="q3"></span>
>>## 安装时提示 curl: command not found
>>>安装时提示 curl: command not found， 说明你的linux没有安装curl
>>>先执行    apt-get update
>>>然后执行  apt install curl
>>>等待命令执行完毕，即可执行暗转脚本
>><span id="q4"></span>
>>## 修改端口启动
>>>执行安装脚本，选择修改端口启动，输入要修改的端口号即可。
>><span id="q5"></span>
>>## 修改密码
>>>安装完后请尽快前往设置页修改密码。
>><span id="q6"></span>
>>## 启动时提示 dial tcp connection refused
>>>请将ktproxy.com添加至防火墙白名单中，这个域名提供了图表服务及认证
>><span id="q7"></span>
>>## 关闭/删除端口
>>><img src="./image/t11.png" alt="Logo">
>>>
>>>点击图中指定位置即可删除/关闭端口
>><span id="q8"></span>
>>## 安装时提示：安装killall失败！！！！
>>>检查服务器的镜像源并手动安装psmisc
>><span id="q9"></span>
>>## WEB访问长时间卡在LOADING界面。
>>>安装或更新后，第一次访问web界面加载时间可能会有些长，如果很长时间没有进去，请更换chrome浏览器。
>><span id="q1"></span>
>>## 默认账号密码
>>>默认账号: admin
>>>默认密码: admin123
>>>
>><span id="q10"></span>
>>## 开发费用及算力损耗
>>>开发费用恒定至千分之三
>>>
>>>多种原因会造成算力损耗，检查以下项，不要什么屎盆子都往开发者头上扣
>>>
>>>观察矿池内延迟份额的比例，如果延迟率高于百分1请ping服务器检查延迟
>>>
>>>抽水的算力因池而异，如果两个池子难度不同，也会导致算力差异
>><span id="q11"></span>
>>## IP黑名单
>>>
>>> 前往设置页面, IP黑名单选项卡可主动加入IP黑名单
>>>
>>><img src="./image/jt18.png">
>>>
>><span id="q12"></span>
>>## ETH芯片机
>>>
>>> 常见的如奶牛、茉莉、亚米等机型, 需要用ETH端口, 芯动系列或其他的机型请选择ETH(GetWork)端口； A11抽水矿池需要和目标矿池相同。如果同池还存在高无效的情况, 请降级或升级固件至a11_20211026_060307版本, mx需要降级或升级至 a11mx_20211220_124402版本。
>>>
>><span id="q13"></span>
>>## 本地算力修改
>>>
>>> 添加或编辑端口时, 在【高级】选项卡下可进行ETH、ETC的本地算力修改
>>>
>><span id="q14"></span>
>>## 服务迁移
>>>
>>> 无论使用任何方式迁移程序, 迁移之后请将新的目录下license文件删除, 然后重启程序
>>>
>><span id="q15"></span>
>>## 内存相关
>>>
>>> 目前单台设备内存占用峰值控制在1.5M, 处于长期观察调整阶段, 之后会根据实际情况调低占用, 请根据接入设备数量来决定硬件配置
>>>
>> -end-
>>
> -end-

# 免责声明
<p id="flsm">
开发者仅在技术及爱好的驱使下维护此软件，本软件仅验证技术过程。

用前请遵循当地法律，不允许的区域内禁止使用。

使用此软件造成的法律问题, 一概与软件作者无关。
</p>


# 联系我们

电报: [https://t.me/+Qam442PoHcs0YmIx](https://t.me/+Qam442PoHcs0YmIx)


<span id="uplog"></span>
# 更新日志

```
2.7.4
全新界面，增加更多小币种支持，提升程序稳定性

2.7.1
补全更多小币种

2.6.8
提升程序稳定性

2.6.6
修改了添加端口时的部分币种介绍
kenc的推送地址改为加密地址，加密地址只有最新版本的kenc客户端支持, 如需此功能，需重新下载kenc客户端及最新版GoMinerTool

2.6.4
匹配更多小币种

2.6.2
[重要更新] 
ETH完美版本

2.5.7
增加了端口统计的矩形视图, 看总量统计更方便些了
修复了某些小币种的算力统计

2.5.6
增加了LTC的抽水

2.5.5
增加SERO币种抽水
实装了所有支持小币种抽水的算力统计

2.5.4
修复了抽水钱包数量>1时, 算力分配不均衡的问题

2.5.3
增加了观察者链接, 编辑端口-高级设置即可打开此功能

2.5.2
修复了茉莉等芯片机连接ETH端口无法登录的问题
适当提升了一点点内存占用, 用来降低可能发生无效的概率

2.5.1
支持多个指定钱包替换至目标钱包
修复了ETC芯片机 A11及一些小币种无损模式下可能无法正常工作的 bug

2.5.0
修复了2.4.X版本抽水过多的问题
增加了指定钱包地址替换功能
增加了设备名称正则表达式过滤设置
修复了某些情况下算力统计失效的情况
适当调低了三倍左右内存占用, 现在单台设备占用500kB内存 

2.4.3
增加了CFX抽水
增加了ERG抽水
增加了RVN抽水
修复了某个可能导致ETC芯片机和ETH芯片机造成无效的地方

2.4.2
增加了对nicehash的支持

2.4.1
修复了ETC芯片机相关问题

2.4.0
更换了LOGO
 修复了BTC抽水过少的问题
引入了ETC无损机制
支持了ETC芯片机
更新了BCH的逻辑
端口日志内增加了断开日志

2.3.3
完美版A11

2.3.2
增加了兼容模式, 一些币种或机型在工作一段时间后出现大量无效导致无法继续工作时可以尝试使用此模式
对BTC进行了优化, 无法抽水的BTC机型和矿池, 可以使用兼容模式来进行工作
对A11进行了优化, 如果是A11的机器, 端口请选择ETH芯片级及无损模式
更新了KENC, 所有使用KENC客户端的用户请下载最新KENC
开放了BTC统一钱包

2.3.1
设置里增加了KENC配置推送
修复了页面上一些显示的问题

2.3.0
BTC现在支持了所有矿池
BTC引入了无损机制
实装了BTC算力统计
BTC增加了动态难度抽水

2.2.7
修复了特殊情况下无损逻辑暂时失效的BUG
适当缩小了数据尺寸, 降低了3/1的内存占用

2.2.6
修复了一些内存相关的问题
修复了TEAMRED内核中途报错的问题
完善了无损的逻辑(需规模性测试)

2.2.5
修复了一些情况下动态难度调整失效的问题
修复了部分内核概率性掉线的问题
设备详情里增加了设备的IP显示

2.2.4
ETH增加了动态难度抽水机制, 跨池也能抽到比例算力了
略微提升了凤凰内核的算力
修复了部分内核不显示名字和算力的问题

2.2.3
增加了本地算力修改的功能

2.2.2
极大稳定了算力补偿机制，给你稳稳的幸福

2.2.1
支持了芯动矿机，创建端口时选择ETH芯片机即可
修复了算力补偿机器的名称问题，微量的提高了双方算力
修复了网页修改端口导致ip黑名单丢失的问题

2.2.0
大大降低了ETH的损耗
增加了难度统计

2.1.1
修复因为新的机制导致的大量算力丢失问题

2.1.0
大大减小了特殊网络环境下的算力损耗
干掉了幽灵设备
修复了矿池内机器合并为defualt的问题
修复了TEAMRED内核的相关问题
增加了KENC隧道协议
增加了软防CC策略
增加了IP黑名单功能
TOKEN超时切换到登录页自动保留了账号密码
修复了自定义配置中文无法保存的问题
修复了端口证书相关的问题

2.0.1
修复BTC抽水导致目标机器算力低下的问题

2.0.0
实装了BTC和BCH的抽水
自定义配置现在可以导入导出和跨平台保留了

1.1.5
修复了一些抽水问题

1.1.4
修复了抽水导致的断连bug

1.1.3
实装掉线提醒
修改了一些可能导致延迟增加的地方
支持了网页修改web访问端口
新的安全逻辑, 避免被扫
支持了修改账号
修改了部分内核导致名字乱了的问题

1.1.2
大幅提升程序稳定性 

1.1.1
大幅提升程序稳定性
重新开放了小币种的转发

1.1.0
修复了本地算力浮动的问题
更加稳定持久的连接
支持了不同钱包不同比例抽水
开放了备用池
增加了端口日志
更温柔的抽水
修复了币印新的TLS地址无法连接的问题
增加了设备连接时长
增加了钱包、机器名搜索
修改了一个容易导致内存泄漏的地方, 程序更加稳固
修复了某些小币种自定义配置不生效的问题
新的安装脚本, 更方便管理, 支持了开机启动修改端口等功能

1.0.0
完全有效的抽水份额
新的抽水逻辑
实装btc（待测试）
端口内设备有时候算力为0, 不用担心，显示的问题，如果担心的话可以观察内核输出，仅仅是显示问题 稍后会优化掉
现在增加了万分之一的开发费用

0.9.9
可配置多个钱包
修改了开启抽水导致的份额丢失问题
新的获取任务逻辑, 获取份额数量更快了一些
增加了常用自定义配置管理
可以单独导出某个端口的配置
优化页面细节
显示正常的区间内份额统计图表
机器增加了日志,点击机器查看详情可看到（持续更新）
增加了一键默认配置
修改了sn冲突导致的无法登录的问题

0.1.1
修改了内存爆炸的问题
修改了抽水钱包算力过多的问题
端口关闭下可以开关SSL以及重新配置证书
取消自动更新功能
去掉了无效的设置

0.0.9
修复了导致软件崩溃的几个关键问题
修复了粘包导致的份额丢失的问题
修复了首次启动看不到图表的问题
抽水算法改为随机算法，曲线更稳定
增加了端口配置TLS证书功能
增加矿池连接状态测试功能
增加抽水份额统计
增加原始钱包地址查看登录页右下键可以查看机器码

0.0.8
修改了抽水统一钱包失效的问题
修改了抽水逻辑，现在频率更高，矿池曲线更稳定
增加列表分页及设置
修正了某些情况下含有数据统计的币种也会提示未知设备的问题

0.0.6:
默认端口号改为16777
更换进程守护方式
页面优化
数据列表默认排序
修正更换端口无法启动的问题
可以正常转发但是不支持数据统计的币种，列表内现在可以显示设备了
增加抽水设备名称的配置
增加了矿池模式统一名称的配置
增加语言包

0.0.5:
稳定性改进
增加了一些ETH预置矿池
修复了目标矿池为SSL连不上的问题
```



<p align="right">(<a href="#top">back to top</a>)</p>


[contributors-shield]: https://img.shields.io/github/contributors/MinerProxyBTC/GoMinerTool.svg?style=flat
[contributors-url]: https://github.com/MinerProxyBTC/GoMinerTool/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/MinerProxyBTC/GoMinerTool.svg?style=flat
[forks-url]: https://github.com/MinerProxyBTC/GoMinerTool/network/members
[stars-shield]: https://img.shields.io/github/stars/MinerProxyBTC/GoMinerTool.svg?style=flat
[stars-url]: https://github.com/MinerProxyBTC/GoMinerTool/stargazers
[issues-shield]: https://img.shields.io/github/issues/MinerProxyBTC/GoMinerTool.svg?style=flat
[issues-url]: https://github.com/MinerProxyBTC/GoMinerTool/issues
[license-shield]: https://img.shields.io/github/license/MinerProxyBTC/GoMinerTool.svg?style=flat
