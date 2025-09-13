# 继承
```
class ChildClass(ParentClass1, ParentClass2):
    # 多继承，用逗号分隔
    pass

空括号（默认继承object）
python
class MyClass:  # 等价于 class MyClass(object):
    pass
```
```
from direct.showbase.ShowBase import ShowBase  # 导入Panda3D的主类

class MyApp(ShowBase):  # MyApp继承ShowBase
    def __init__(self):
        ShowBase.__init__(self)  # 调用父类的构造函数
        # 这里可以添加自定义初始化代码

app = MyApp()  # 创建MyApp实例
app.run()      # 运行游戏循环
```
**python里要给父类构造，同时构造函数需要写self**
