# 模块化设计

一个完整的ThinkPHP应用基于**模块/控制器/操作**设计，并且，如果有需要的话，可以支持多入口文件和多级控制器。

ThinkPHP新版采用模块化的架构设计思想，对目录结构规范做了调整，可以支持多模块应用的创建，让应用的扩展更加方便。

一个典型的URL访问规则是（我们以默认的PATHINFO模式为例说明，当然也可以支持普通的URL模式）：

http://servername/入口文件/模块/控制器/操作方法

http://www.tp5.com/index.php/index/user/showUser



