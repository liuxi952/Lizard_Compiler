# Lizard Compiler

## 中文

Lizard Compiler 是一个基于 C++ 实现的简易编译器项目，用于演示“词法分析、表达式解析、字节码生成与虚拟机执行”这一类编译器基本结构。

这个项目最初是一个教学型内测版本，当前已经具备了基本的脚本执行能力，适合用于学习编译器原理以及简单语言的编译/运行流程。

## 项目特点

- 支持输出语句 print
- 支持变量定义与赋值
- 支持基本算术表达式：+、-、*、/
- 支持比较表达式：>、<、>=、<=、==、!=
- 支持字符串常量
- 支持 if / else 分支
- 支持 while 循环
- 支持 ++ / -- 自增自减
- 支持 return 语句
- 支持通过 .cl 脚本文件运行

## 示例代码

```cl
int i = 0
while(i < 2) {
    i++
}
print i
```

另一个简单示例：

```cl
int a = 3
int b = 5
print a + b
print "Hello, Lizard!"
```

## 项目结构

- Lizard/Lizard/Lizard.cpp：主程序、词法分析、语法编译、虚拟机执行逻辑
- Lizard/test.cl：示例脚本文件

## 如何运行

1. 你可以直接在文件夹里直接运行可执行文件，并传入一个 .cl 脚本文件：

```bash
Lizard.exe test.cl
```

如果你想注册 .cl 文件关联，也可以使用：

```bash
Lizard.exe --register
```

## 说明

当前版本仍属于轻量级编译器，重点在于展示基本实现思路，后续可以继续扩展为更完整的脚本语言，例如：

- 函数定义与调用
- 更多的数据类型
- 更完善的语法错误处理
- 更丰富的控制流支持

## English

Lizard Compiler is a lightweight C++-based scripting compiler project designed to demonstrate the fundamental structure of an compiler, including lexical analysis, expression parsing, bytecode generation, and virtual machine execution.

This project started as a teaching-oriented internal preview version. It already supports basic script execution and is suitable for learning compiler principles, virtual machine design, and the basic workflow of compiling and running a simple language.

## Features

- Supports print statements
- Supports variable definition and assignment
- Supports basic arithmetic expressions: +, -, *, /
- Supports comparison expressions: >, <, >=, <=, ==, !=
- Supports string literals
- Supports if / else branches
- Supports while loops
- Supports ++ and -- increment/decrement operations
- Supports return statements
- Supports running scripts from .cl files

## Example Code

```cl
int i = 0
while(i < 2) {
    i++
}
print i
```

Another simple example:

```cl
int a = 3
int b = 5
print a + b
print "Hello, Lizard!"
```

## Project Structure

- Lizard/Lizard/Lizard.cpp: main program, lexical analysis, syntax compilation, and virtual machine execution logic
- Lizard/test.cl: example script file

## How to Run

1. You can run the executable directly in the folder and pass in a .cl script file:

```bash
Lizard.exe test.cl
```

If you want to register .cl file association, you can also run:

```bash
Lizard.exe --register
```

## Notes

The current version is still a lightweight compiler focused on demonstrating core implementation ideas. It can be extended in the future to support a more complete scripting language, such as:

- Function definitions and calls
- More data types
- More robust syntax error handling
- Richer control flow support
