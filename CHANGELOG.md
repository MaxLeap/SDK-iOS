2.0.10 发布日期：2016-5-16

**新增**

新增 `MaxSocial` 和 `MaxSocialShare` 两个模块 </br>
`MaxSocial` 用来支持一些常用社交功能，包括注册登录、关注、发表说说、评论等</br>
`MaxSocialShare` 聚合了微信朋友圈、微信好友、QQ好友、QQ空间、新浪微博分享接口，并且支持扩展</br>

`MaxIMLib`: 可以给 user,group,room 设置自定义属性，新增查询功能，新增游客登录模式</br>

修复一些 bug


2.0.9 发布日期：2016-3-29

支持微信支付和银联支付</br>
支持实时通信</br>
支持 QQ 登录</br>
MLObject 子类支持实例变量


2.0.7 发布日期：2016-01-11

新特性：MaxPay，集成支付宝支付功能和订单查询功能</br>
bug 修复

2.0.6 发布日期：2015-12-30

新特性：第一次打开应用以及用户登出后自动创建匿名用户</br>
修复若干 bug

2.0.5 发布日期：2015-12-14

增加短信验证功能接口</br>
支持微博微信登录

2.0.4 发布日期：2015-12-11

MLObject 支持 KVC `setValue:forKey`，但是暂不支持 KVO</br>
修正一些注释</br>
修复行数据中存储的文件链接为空时，SDK 会崩溃的问题</br>
修复 MLObject 子类跟 子类的子类可以拥有不同的 leapClassName 的问题</br>
其他 bug 修复

2.0.3 发布日期：2015-11-23

修复删除服务器上的 config 后，本地缓存不删除对应的 config 的 bug</br>
添加 nullability annotations

2.0.2 发布日期：2015-11-03

识别新设备(iPhone6s, iPhone6s Plus, iPod touch 6G, iPad Pro)</br>
修复应用开启 bitcode 后无法打包的问题</br>
重新设计 MLLogger

2.0.1 发布日期：2015-10-21

修复应用连接 MaxLeap SDK 使用 Xcode 7 编译时会报警告的问题

2.0.1-pre 发布日期：2015-10-16
