同步twitter到新浪微博
====================

部署在Google Appengine上，自动同步twitter到新浪微博，自动转换短链接以防止被屏蔽，自动同步twtter消息中flickr、Instagram、twitter等网站的图片。

安装
---

安装需要以下几步。

* 申请一个[tiny.cc](http://tiny.cc)的帐号。从api页面[http://tiny.cc/api-docs](http://tiny.cc/api-docs)取得你的API Key
* 在新浪微博开放平台http://open.weibo.com/申请成为开发者。注意，要用你想要同步的微博帐号申请。
* 创建一个应用。类型可以选为网页应用。在该应用的控制台页面取得应用的App Key。
* 编辑myid.py文件，把用户名密码和申请到的App keys填入。注意，除了weibo apikey直接填数字，其他都是string类型，直接填写在双引号中。

     my_twitter_id=""
     my_weibo_username=""
     my_weibo_password=""
     my_weibo_apikey=1234567890
     my_tinycc_login=""
     my_tinycc_apikey=""


部署
---

更改app.yaml中的application id，上传到Google App Engine上。

部署到Google App Engine就是通常的app engine流程，可参看下面两个教程。

* [Google App Engine 入门:上传应用程序](http://blog.xuming.net/2008/05/google-app-engine-toturial-9.html)
* [Google App Engine 6步上手教程](http://www.cnblogs.com/2011sydney/archive/2009/07/23/1529637.html)


示例
---

这是我建的一个Lady Gaga的同步。Lady Gaga [twitter](), Lady Gaga [微博](http://weibo.com/u/2841791740)

License
-------
GPLv3 [gplv3]
参考:http://code.google.com/p/twitter-feed/
     http://atlee.ca/software/poster/


[gplv3] [http://www.gnu.org/licenses/gpl.html]