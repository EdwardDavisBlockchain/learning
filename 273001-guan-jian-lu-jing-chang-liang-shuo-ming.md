# 关键路径常量说明

1. THINK\_VERSION 框架版本号
2. DS 当前系统的目录分隔符
3. tp5 项目根目录 ROOT\_PATH
4. tp5/application 应用目录 APP\_PATH
5. tp5/thinkphp 框架核心目录 THINK\_PATH
6. tp5/exend 应用扩展目录 EXTEND\_PATH
7. tp5/vendor Composer扩展目录 VENDOR\_PATH

```php
<?php
namespace app\index\controller;

class Index
{
    public function index()
    {
        return 'hello world';
    }

    public function showConst()
    {
    	echo "TP5的版本号".THINK_VERSION."<br>";
    	echo "TP5的目录分割符".DS."<br>";
    	echo "TP5的根目录".ROOT_PATH."<br>";
    	echo "TP5的核心目录".THINK_PATH."<br>";
    	echo "TP5的应用程序目录".APP_PATH."<br>";
    	echo "TP5的扩展目录".EXTEND_PATH."<br>";
    	echo "TP5的第三方目录".VENDOR_PATH."<br>";
    }
}
```

#### 结果：![](/assets/import27.png)



