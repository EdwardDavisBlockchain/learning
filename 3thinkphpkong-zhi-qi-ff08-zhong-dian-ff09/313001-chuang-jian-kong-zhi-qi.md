# 创建控制器

ThinkPHP 5 的控制器比较灵活，可以不用继承任何基础类，也可以继承官方封装好的 \think\Controller 类或者其他的控制器类

#### 方法一：定义一个控制器（不继承任何基础类）

![](/assets/import28.png)

首先在controller文件夹下新建一个文件 注意文件名首字母要大写且以.php结尾

创建好之后我们开始在文件里写入代码：

```php
<?php
namespace app\index\controller;
class User{
    function showUser(){
        return "这是我的第一个自定义控制器";
    }
}
```

#### ![](/assets/import29.png)方法二：定义一个控制器继承父类

还是先创建文件只不过文件里的代码不同

```
<?php
namespace app\index\controller;

use think\Controller;
class User extends Controller{
    function showUser(){
        return "这是一个继承父类的控制器";
    }
}
```

### ![](/assets/import30.png)小结：

**Q：创建控制器是否引用父类并继承父类？**

**A：最好继承父类**

**Q：怎样输出运行的结果？**

**A：建议统一使用 return 返回数据，而不是 echo 输出，如非必要，请不要使用exit或者die中断执行。直接echo输出的数据将无法进行自动转换响应输出。**

**Q：TP5是如何响应输出的？**

**A：控制器的所有操作方法都是 return 返回而不是直接输出，系统会调用Response::send方法将最终的应用程序发送处理，底层开发文件是：**

![](/assets/import31.png)

![](/assets/import32.png)

![](/assets/import33.png)

> 返回的数据输出到页面或者客户端，并自动转换成 default\_return\_type=html 参数配置的格式。所以，应  
> 用执行的数据输出只需要返回一个正常的PHP数据即可



