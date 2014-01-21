WeixinRouter
============

一个微信转发服务器。把微信公众平台高级开发接口的XML格式，转换为POST参数形式。另外数据返回统一使用JSON格式。
方便接口的开发和调试。

功能说明
=======
*  支持不同功能使用统一的入口， APP/USER/SESSION
*  支持接口统计功能
*  支持友好的错误提示，应用接口超时。会返回微信客户端信息。
*  支持多个应用接口集成。



路由规则配置
==========

例子:
```bash
route -A input -type text -content liu -j forward -app_type xml -app_url http://wx2.emop.cn/route/51/3000052/1357 -app_token cb05694fd559dcfbacbac57ae2547733
route -A input -type text -content liu -j forward -app_type json -app_url http://emopselljd.sinaapp.com/api/wx_reply -app_token cb05694fd559dcfbacbac57ae2547733
```