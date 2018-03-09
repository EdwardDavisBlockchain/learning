# 获取ThinkPHP5.0

#### 方式一：直接在官网上下载最新版本的TP5框架

#### ![](/assets/123.png)方式二：使用git版本库安装

首先克隆下载应用项目仓库：git clone [https://github.com/top-think/think](https://github.com/top-think/think) tp5

然后**切换到 tp5 目录**下面，再克隆**核心框架**仓库： git clone [https://github.com/top-think/framework](https://github.com/top-think/framework) thinkphp

![](/assets/321.png)

![](/assets/QQ截图20180309130758.png)

#### 下载完成目录

![](/assets/QQ截图20180309130933.png)

![](/assets/QQ截图20180309131105.png)

#### 方式三：composer安装

> Composer不是一个包管理器。是的，它涉及"packages"和"libraries"，但它在每个项目的基础上进行管理，在你项目的某个目录中（例如vendor）进行安装。默认情况下它不会在全局安装任何东西。因此，这仅仅是一个**依赖管理**。**就是解决软件依赖的一个软件。**

* composer安装步骤这里不做过多阐述，请自行百度

composer安装完成之后 进入cmd命令窗口将目录地址切换到你要存放TP5框架的目录

![](/assets/import.png)![](/assets/import1.png)

开始执行命令：**composer create-project topthink/think tp5 --prefer-dist**

![](/assets/import2.png)

![](/assets/import4.png)

* 注意我在第二张图里面将路径更换为  **E:\Thinkphp\mytp5**



