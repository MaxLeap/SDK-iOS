2.1.3 发布日期：2016-09-28

MaxLeap

- 删除 SSKeychain
- 修复一些问题

MaxIM

- 兼容 socket.io-client-swift v8.x (使用 swift3)
- 添加新的错误码 kMLIMErrorInvalidQuery
- 修复 message.attachmentUrl 总返回空的问题

MaxSocial

－ MaxSocialShuoShuo 添加一个新的字段 `share`，可用来保存自定义数据

2.1.2 发布日期：2016-09-09

MaxLeap

- Installation 增加 sandbox 字段，用来标记是否是推送测试环境
- MLUser 增加 mobilePhone 和 mobilePhoneVerified 属性
- MLObject 禁止对声明为 readonly 和 dynamic 的属性执行 -setObject:forKey: 方法
- 修复了多次调用同一个 MLObject 的保存方法偶有数据丢失的问题
- 修复 In-App Message 下载出错的问题
- 修复 In-App Message 会重复展示多次的问题

MaxIM

- MLIMMessage 增加了与推送定制相关的属性 pushxxx
- MLIMMessage 增加了 remark 字段，可以存放自定义消息结构
- MLIMClientConfiguration 增加 voip 开关
- 新增陌生人聊天方式
- 修复使用除UserId登录以外的登录方式登录收不到离线推送消息的问题
- 修复偶尔会 crash 的问题

2.1.1 发布日期：2016-8-19

MaxLeap

- 优化在SDK初始化之前调用 `[MLUser user]` 或者 `[MLInstallation currentInstallation]` 抛出的异常信息
- 修复网络请求内存泄漏的问题

MaxSocial

- 增加批量创建／更新评论的接口
- 更新获取未读评论的接口
- 修复说说图片顺序与上传顺序不一致的问题

MaxIMLib

- SocketIOClientSwift 升级至 v6.1.6
- MLIMClientConfiguration 新增 baseURL 属性，用来更改服务器地址
- MLIMFriendInfo 升级为可扩展的类
- 其它错误修正

2.1.0 发布日期：2016-6-24

**重大变更：**

- `MLHelpCenter` 开源，并且拆分为 [MaxFAQ](https://github.com/MaxLeap/Module-MaxFAQ-iOS) 和 [MaxIssues](https://github.com/MaxLeap/Module-MaxIssues-iOS), `MLHelpCenter.embeddedframework` 以后不再与 `MaxLeap.framework` 一起发布
- `MaxIMLib.framework` 改为静态库，原动态库更名为 `MaxIMLibDynamic.framework`
- `MaxSocial` 原来的评论创建方法变更为：`- (void)createOrUpdateComment:(NSDictionary *)params block:(MLSCommentResultBlock)block;`， 老方法可能失效

其他更新：

- 修复了对 MLObject 子类的子类必须显式声明遵循协议 `MLSubclassing` 的 BUG
- 修复了在32位机器上，BOOL 类型的属性值会被序列化成数字的 BUG


2.0.10 发布日期：2016-5-16

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
