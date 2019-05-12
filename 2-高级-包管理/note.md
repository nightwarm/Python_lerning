# 1.模块
- 一个模块就是一个包含python代码的文件，后缀名是.py就可以，模块就是个python文件
- 为什么用模块
    - 程序太大，编写维护非常不方便，需要拆分
    - 模块可以增加代码重复利用的方式
    - 当作命名空间使用，避免命名冲突
- 模块定义
    - 模块就是一个普通文件，所以任何代码都可以直接书写
    - 不过根据模块的规范，最好再模块中编写以下内容
        - 函数（单一功能）
        - 类（相似功能的组合，或者类似业务模块）
        - 测试代码
- 如何使用模块
    - 模块直接导入
        - 加入模块名称直接以数字开头，需要借助于importlib的帮助
    - 语法
        import module_name 
        module_name.function_name
        module_name.class_name
        - 案例 01，02，p01，p02
    - import 模块 as 别名
        - 导入的同时给模块起一个别名
        - 其余用法同第一种
        - 案例p03
    - from module_name import func_name,class_name
        - 按上述方法有选择性的导入
        - 使用的时候可以直接使用导入的内容，不需要前缀
        - 案例 p04
    - from module_name import *
        - 导入模块所有内容
        - 案例p05