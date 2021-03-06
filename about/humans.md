# 规范

本文将分为三方面:

- [规范](#规范)
  - [文件结构规范](#文件结构规范)
  - [代码规范](#代码规范)
    - [代码](#代码)
    - [命名](#命名)
    - [注释](#注释)
  - [协作流程规范](#协作流程规范)
  
:dog:

## 文件结构规范  

[新手程序员开发项目规范](https://zhuanlan.zhihu.com/p/161640510)

文件目录结构如下图：
![文档目录结构](/assets/img/dirctorystructure.png)  

## 代码规范

本项目开发使用python为主，因此代码规范非常重要，借鉴 [Google Style Guide](https://github.com/google/styleguide/) 后，将python代码规范分为以下三点加以说明。

- 代码
- 命名
- 注释

### 代码

格式化代码方式选择：yapf;

避免全局变量;

坚决不在行尾使用分号;

每一行最大长度为80（例外如下）：

- 长的导包语句
- URL，路径名

采用4空格缩进；

### 命名

变量 local_var_name;
类名 ClassName;
方法名 method_name();
函数名 function_name;
常量名 CONSTANT_NAME;
函数参数名 function_parameter_name;
模块名 module_name(self defined);

**注意**:angry:
除循环与迭代器外禁用单字符名称；
"__"双下划线开头的实例变量或方法表示类内私有；
"_"命名连接的前后两部分要有逻辑关系避免var_1,var_2这样的命名——尽量赋予变量名称以实际意义；

### 注释

鉴于本项目比较初级，创建新类新文档新函数的概率不大，故此处只展示单行注释以及行内注释的规范。
（如涉及到行间注释则更新规范文件）

原则：

- 行内注释仅发生在核心公式与核心迭代算法后；
- 行内注释在能表达意思的情况下越短越好；
- 行内注释离开代码统一规定为8个空格；
- 永远假设读者比你更懂python，只解释意图不解释语法；

## 协作流程规范

统一使用GitHub Desktop进行项目协作，win10下vscode与ubuntu下gedit为主要编辑器。

协作要求：

- 修改文档可以直接请求在main分支上合并
- 修改代码只允许新建分支，经二人均同意后方可合并入main
