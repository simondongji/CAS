# SSO [![Build Status](https://travis-ci.org/laomazi2006/sso.svg?branch=master)](https://travis-ci.org/laomazi2006/sso) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/laomazi2006/sso/master/LICENSE) [![GitHub issues](https://img.shields.io/github/issues/laomazi2006/sso.svg)](https://github.com/laomazi2006/sso/issues)

打造一个单点登录平台，其中包括以下子系统

* CAS SERVER
* 配置中心
* 服务管理系统
* 监控平台
* 客户端集成(cas client、pac4j、shiro)

并且在博客中记录整个大家过程以及注意事项

--------------------

其中每一个阶段会发布一个版本，里程碑为：

1. CAS搭建HelloWorld
2. SSL证书生成并导入https
3. 配置中心搭建
4. cas-management搭建
5. 监控平台搭建
6. CAS数据库认证，密码管理
7. 多属性返回
8. 自定义主题
9. 授权码持久化配置、票据持久化配置
10. CAS多系统安全
11. CAS client demo测试单点登录
12. Pa4j客户端单点登录整合
13. Rest协议认证
14. Shiro代理认证
15. OAuth协议对接


## Tutorial: [![Csdn Blog Tutorial](https://img.shields.io/badge/csdn%20blog-tutorial-orange.svg)](http://blog.csdn.net/u010475041/article/category/7156505)

* [Blog](http://blog.csdn.net/u010475041/article/category/7156505)
* [Support](https://github.com/laomazi2006/sso/wiki)

域名：passport.sso.com

用户：

| 用户名 |密码|是否可登录|备注|
|:-------|:-------|:-------|:-------|
|admin|123|√||
|zhangsan|12345678|√||
|zhaosi|12345|×|禁用|
|wangwu|1234|√|需修改密码|

## 模块介绍


| 模块名 |模块介绍|端口情况|必须https|path|启动循序
|:-------|:-------|:----|:-------|:-----|:--|
|sso-server|cas服务|8443|√|cas|2|
|sso-config|配置中心|8888|×|config|1|
|sso-management|service管理|8081|×|cas-management|3|
|sso-cas-client-demo|cas-client-demo|8080|×|/sample|4|
|sso-client-shiro-demo|shiro-client-demo|8083|×|/|5|

## 代码下载 [![码云](https://img.shields.io/badge/download-码云-yellowgreen.svg)](https://git.oschina.net/Kawhi-Carl/sso) [![Github](https://img.shields.io/badge/download-GitHub-brightgreen.svg)](https://github.com/laomazi2006/sso)

1. 每一个阶段都会封版打一个tag，需要的进行[下载](https://github.com/laomazi2006/sso/releases)
2. 原始构建文件存在于original-files目录下

## Development [![Dependency Status](https://www.versioneye.com/user/projects/59b6afd60fb24f004e1a656b/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/59b6afd60fb24f004e1a656b) <!-- [![Dependency Status](https://dependencyci.com/github/laomazi2006/sso/badge)](https://dependencyci.com/github/laomazi2006/sso)  -->[![codebeat badge](https://codebeat.co/badges/4b430ffd-0cb8-4310-b081-955a66e65c76)](https://codebeat.co/projects/github-com-laomazi2006-sso-master)

* jdk8
* maven3

