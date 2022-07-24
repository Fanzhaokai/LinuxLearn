# 服务器概述
## 公网ip和私网ip
公网ip就是外界访问的，私网ip自己访问的
## root 用户
当我们购买好一个服务器之后，可以重置密码，这个密码可以用来在xshall登录
![在这里插入图片描述](https://img-blog.csdnimg.cn/5a289aeff50c4fda8eda88d93d97238f.png)
## xshall链接
点击文件-》新建
![在这里插入图片描述](https://img-blog.csdnimg.cn/54a5e1895416494888b3ec62f5f8c167.png)
名称可以随便填
在主机号位置，写入购买服务器时的公网ip然后点击确认

![在这里插入图片描述](https://img-blog.csdnimg.cn/8b86630e30554c75afda5de5135ca833.png)
点击确认后，所有会话这一栏下面就有刚刚创建的的连接。
双击它，就进入登陆页面了
![在这里插入图片描述](https://img-blog.csdnimg.cn/bfa877f947c541ab9c8d7bd5adf9d0d3.png)
** 注意**
在第一次登陆的时候，我们的用户名是 root，因为在linux中，root是管理员的意思。
![在这里插入图片描述](https://img-blog.csdnimg.cn/fbd02997d2a64f928c23b2a194d151f6.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/2ea33aee629c402f92d38799a8adbe6d.png)
密码就是我们服务器重置密码后的新密码
![在这里插入图片描述](https://img-blog.csdnimg.cn/765b842c03d84dedbee283f3b1402961.png)
出现这里时表示成功登录
# Linux命令概述
## 创建用户

```csharp
adduser zhangsan
```
表示创建一个用户（必须在root），用户名叫 zhangsan之下。这时会我们的一个用户就创建完成了。
```
passwd zhangsan
```
这里表示修改zhangsan的密码
![在这里插入图片描述](https://img-blog.csdnimg.cn/27ca2af50aa44b27b557fdecf73d5d09.png)
 输入一次后会提示retry，再输入一次即可
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/1767887d64114308a66ec8a457f6718c.png)
 当出现如下时，说明用户已经创建成功
 ## 退出用户
 输入**exit** 即可退出
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/ad159c15bc3d436e9b99aaab00dbc40b.png)
 当出现以上情况时，说明推出成功。接下来我们可以用zhangsan用户来登录服务器了。
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/c4db73350aa84d4f8b9319d04e706666.png)
 按照登录步骤再来一遍，就可以用zhangsan这个用户登陆了。
 
 ## 查看当前用户
 ```
 whoami
 ```
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/6179dfc392fe44a1a7b81a800c9cf8dd.png)
## 查看所有用户
```
ls /home
```
![在这里插入图片描述](https://img-blog.csdnimg.cn/ed9eba5ff608480cab8278546aeb5037.png)
注意查看所有用户只能在root下运行

 ## 删除用户
 ```
 userdel -r zhangsan
 ```
 注意删除用户只能在root用户下使用

 ![在这里插入图片描述](https://img-blog.csdnimg.cn/0bd246343c7440be80bf5eabe1a34068.png)
 
 














