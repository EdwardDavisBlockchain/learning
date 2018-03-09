# 控制器的命名规范

了解过tp3.2.X版本的小伙伴们应该知道 在tp 3 版本中控制器的命名规范是：控制器名称+Controller+.php

![](/assets/import34.png)

但是在我们TP5中 Controller 不是必须的 格式为：**控制器名称+.php（控制器名称首字母大写）**

![](/assets/import35.png)

那么问题来了 我熟悉了tp3的控制器写法了 该怎么办呢？ 别着急 tp5也可以写 控制器名称+Controller+.php的格式但是要在配置文件中更改配置

![](/assets/import36.png)

![](/assets/import37.png)

将参数 false 修改为 true 那么就可以使用 控制器名称+Controller+.php的格式了![](/assets/import38.png)![](/assets/import39.png)

