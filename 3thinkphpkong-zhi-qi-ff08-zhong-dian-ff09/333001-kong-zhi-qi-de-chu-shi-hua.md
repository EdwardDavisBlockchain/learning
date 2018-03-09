# 控制器的初始化

如果你的控制器类继承了\think\Controller类的话，可以定义控制器初始化方法\_initialize，在该控制器的方法调用之前首先执行。

```php
<?php
namespace app\index\controller;

user think\controller;
class User extends Controller{
    public function _initialize(){
        return "我会出现在最前面---------";
    }

    public function showUser(){
        return "演示控制器初始化方法";
    }
}
```

![](/assets/import40.png)

