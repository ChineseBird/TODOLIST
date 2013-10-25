1. app执行的跳转回的URL不能与鉴权服务器www.yilos.com域名重复
2. node fore的children无法做session负载均衡需要session集中处理
3. 在注销请求中需要先将request的session清空，否则最后一个回请求会产生一个新的session导致session泄露
4. 认证登陆界面js错误导致，没有设置用户名到客户端，导致无法注销用户的session
5. 客户端token超时时间设置为一年
6. 服务端session超时时间也需要设置一年(只针对app，因为app长期不退出)
4. 店铺信息和账号信息需要个更新
5. 没有网络的情况下的错误提示要友好
