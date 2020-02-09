# Dog Tunnel(狗洞新版)
- [ ] 改用rust重写，集成p2p和lite版本的所有功能
- [ ] 支持upnp
- [ ] 支持本地udp固定端口
- [ ] 支持stun标准化服务
- [ ] 多端口映射
- [ ] 方便的动态配置
- [ ] nats类型检测
- [ ] 支持限速
- [ ] 账号认证
- [ ] connection抽象，可a到b，可a到c到b,中间可加filter支持脚本
- [ ] 静态单文件部署
- [ ] 方便清晰的归类配置

不保证开发进度



为什么要用rust？

- 一直想用
- 做一些技术考察，后期公司项目可能会引入
- 可更方便的进行cpu和内存精确控制
- 最初狗洞为了挖矿远程操作用，很多都是临时写写的，不想在上面重构了，直接重写

会鸽吗？

​	不保证，现在也是有娃的人了，时间对我来说是非常宝贵的东西，所以项目前期会持续开发，但是不保证时间。

为什么要重写

​	狗洞作为第一款kcp的开源应用，可能并不为大多数人所知，p2p版本是我为了远程连回家中btc矿机所写，而lite版本为后期科学上网所写，很多时候只是满足自己的一些临时想法的实现，所以并没有做太多的设计，其实lite版本作为稳定服务已经在我的pi和网关以及vps上跑了1-2年以上，几乎从未重启。因为疫情的原因，导致最近犯了一些代码洁癖，加上又有了一些新的想法，所以萌生了重写的念头。