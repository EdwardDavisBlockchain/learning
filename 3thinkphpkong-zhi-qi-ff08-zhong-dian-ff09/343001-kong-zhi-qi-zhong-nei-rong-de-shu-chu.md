# 控制器中内容的输出

无论在那个框架里，输出都是尤为重要的 更何况对API这么友好的TP5

输出数组：可以使json格式

Q：怎么将数组转化为json格式

A：方法一：在配置文件里面配置

![](/assets/import41.png)

方法二：使用助手函数json\(\)来输出json格式

```php
<?php
namespace app\index\controller;

use think\Controller;
class User extends Controller{
    function _initialize(){
        echo  "我会出现在最前面---------";
    }

    public function showUser(){
        $arr = [5=>'1','2','3'];
        return json($arr);
    }
}
```

![](/assets/import42.png)



