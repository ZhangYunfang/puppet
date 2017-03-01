扯线木偶（puppet）

主旨：将同花顺交易客户端、通达信历史行情数据和预警功能、腾讯实时行情数据以及自建的策略（择时/选股/交易/风控）组合成闭环的程序化交易系统。

工作流程：手动登录客户端 --> 运行扯线木偶 --> 自动搜索已登录的客户端 --> 交易前的预备 --> 自动获取持仓数据 --> 查询预警名单 --> 客户端待命状态

推荐使用最新版的Anaconda3，或者Python >= 3.5。

2017/2/23 V0.3.5发布！小幅修改，改善操作流畅度。

2017/2/22 v0.3发布！优化模拟人手交易的流程。

2017/2/21 v0.2.5发布！增加撤单（指定股票代码）功能。

2017/2/14 v0.2版发布！提供后台获取持仓数据。鸣谢网友liuyukuan博文中提供的AHK代码“SendMessage,0x111,57634,0,CVirtualGridCtrl2,同花顺”。

Windows下不需要安装、配置。

Linux下需要安装最新版本的Wine，环境设为Windows 7，先安装同花顺交易客户端，能正常使用之后再安装Python for Windows。启动wineconsole，pip install pyperclip，之后就可以正常使用了。

1、支持同花顺的“所有”交易客户端：官方统一版或老版、券商定制版（银河、国泰君安、华泰、广发、东方财富等）。

2、支持多种交易模式：同一券商多个账户、多个券商多个账户同时登录一个（或多个）交易端，并且同时进行交易。

3、目前仅支持多个不同的交易客户端登录后同时交易，暂时不支持一个交易客户端多个账户登录后同时交易。

下一步计划：精简交易行为逻辑，重构新版本，支持同一股票多账户并发下单、多账户自动登录、掉线重登陆。
