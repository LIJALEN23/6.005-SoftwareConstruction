# 静态类型与软件三大优秀特性

## Types类型
- Java分为基本类型和引用类型
- Java运算符与重载

## Static typing静态类型
- 静态类型语言：如Java，在编译时确定所有变量的类型(编译器就可以推断出很多bug)
  - 动态类型语言：如Python(在高版本之后拓展了静态类型)，在程序运行时才确定

## Static checking, dynamic checking, no checking静态检查、动态检查、不检查
- 静态：编译之前检查
  - 语法错误
  - 名称拼写错误
  - 参数数量错误
  - 错误参数类型
  - 返回类型错误
- 动态：程序运行时检查
  - 非法参数值
  - 非法转换
  - 超出索引
  - null对象上调用方法
- 无：语言无法检查

## Arrays and collections数组和集合
- 一般不使用定长的数组：可能造成缓冲区溢出

## Iterating迭代
- 遍历一个集合

## Method方法
- 方法的使用范围、静态方法、方法文档

## Mutating values vs. reassigning variables
- 应尽量避免变化的事情发生
- final和不可变类型

## Documenting assumptions记录假设
- 记录下变量的假设范围
  - 使编译器自动检查
  - 使其他程序员知道

## Hacking vs. engineering黑客与工程
- hacky code：
  - 在测试前编写大量代码
  - 记住程序所有细节(几乎不可能)
  - 忽略bug的危害
- engineers are pessimists：
  - 编写代码边测试
  - 记录代码的细节
  - 避免小细节错误

## Goal of this course这个课程的目标
- Safe from bugs：软件要有安全性和防御性
- Easy to understand：即可读性
- Ready for change：更新等等
- Else：性能、可用性

Java的特性
- 安全
- 流行