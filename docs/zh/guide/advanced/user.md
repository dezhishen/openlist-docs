---
# This is the icon of the page
icon: iconfont icon-people
# This control sidebar order
order: 2
# A page can have multiple categories
category:
  - Guide
# A page can have multiple tags
tag:
  - Advanced
  - Guide
# this page is sticky in article list
sticky: true
# this page will appear in starred articles
star: true
---

# 用户

## **用户名**

登录用户名

## **密码**

登录密码

:::tip
密码对游客是无效的，

如果连续输入6次密码错误会对当前IP封禁30分钟无法输入账号密码登录，但是不会影响其它IP，只针对输入6次密码错误的IP

- 重启可立刻消除30分钟封禁时间

:::

<br/>



## **基本路径**

用户登录时看到的根路径

-----

Q：**如何否允许一个用户可以看到多个文件夹路径?**

A：可以新建一个[别名](alias.md)存储,将你需要给用户展示的路径都添加到别名，然后在用户路径这里指向新建的别名存储

<br/>



## **权限**

- 可以看到隐藏：可以看到隐藏的文件和文件夹
- 无密码访问：无需密码即可访问
- 添加离线下载任务：添加离线下载任务
- 创建目录或上传：可以创建目录或上传文件
- 重命名：可以重命名文件和文件夹
- 移动：可以移动文件和文件夹
- 复制：可以复制文件和文件夹
- 删除：可以删除文件和文件夹
- WebDAV 读取：可以使用 WebDAV 读取文件和文件夹
- WebDAV 管理：可以使用 WebDAV 管理文件和文件夹
- FTP 读取：可以使用 FTP 读取文件和文件夹
- FTP 管理：可以使用 FTP 读取文件和文件夹
- 读取压缩文件：读取压缩包内的文件内容
  - 打开此选项后，默认会对压缩包格式文件进行预览(如下图所示)，会消耗一些服务器流量，但不会全部下载
  - 如果要关闭压缩包格式首选预览，==**后台 => 设置 => 打开压缩包文默认预览**==，此选项关闭，首选项就是下载模式

- 解压：在线解压压缩包文件

![](/img/advanced/user_read_archives_light.png#light)

![](/img/advanced/user_read_archives_dark.png#dark)

<br/>



## **停用**

勾选后将停止使用此用户，无法登陆，游客账户默认停用，如果要启用游客账户请手动关闭停用

<br/>



## **Tips**

1. 你是否在为游客能看到全部文件而发愁？[**点击查看这里如何设置**](../../faq/why.md#%E6%83%B3%E8%AE%A9%E6%B8%B8%E5%AE%A2%E7%99%BB%E5%BD%95%E5%90%8E%E6%89%8D%E8%83%BD%E7%9C%8B%E5%88%B0%E5%86%85%E5%AE%B9%E6%80%8E%E4%B9%88%E8%AE%BE%E7%BD%AE)
2. **`Guest user is disabled, login please`**：为了保护您的OpenList安全，游客访问权限关闭了，若需要游客访问自行打开
   - 后台 --> 用户 --> `guest` --> 停用取消勾选
3. 关于 **`复制/上传`** 的问题
   - 如果你上传(含离线下载上传)很大的文件，或者上传文件很多（几百上千），不建议您使用OpenList来进行操作,请前往相应的网盘官网直接操作最后
4. 非admin权限用户在后台管理离线下载、复制、上传等操作
   - 需要OpenList升级到<Badge text="v3.39.1" type="info" vertical="middle" />版本，同时admin也可以查看用户的任务进度以及操作

![](/img/advanced/user_manage.png)

