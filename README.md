# README
## This document written by markdown will record the road of my progress.

* Firstly, I want to write something. BUT! I think I suppose to give a brochure to tell me how to write this document by markdown.

# markdown格式

## 标题

* \# 一级标题
* \## 二级标题
* \### 三级标题
* \#### 四级标题
* \##### 五级标题
* \###### 六级标题 

### 格式显示

* # 一级标题

* ## 二级标题

* ### 三级标题

* #### 四级标题

* ##### 五级标题

* ###### 六级标题

* 正文格式







## 段落格式

### 换行

添加两个以上的空格后回车





## 字体格式

* 斜体格式
  * \*斜体文本*
  * \_斜体文本_
* 粗体格式
  * \**粗体文本**
  * \__粗体文本__
* 粗斜体格式
  * \*\*\* 粗斜体文本\*\*\*
  * \_\_\_粗斜体文本\_\_\_

* 分隔线
  * \***
  * \---

* 删除线
  
* \~~带删除线的文本\~~
  
* 下划线
  
* <u> 带下划线的文本</u>
  
* 脚注

  * 创建脚注格式类似这样[^little_chai]

  * [^little_chai]: 小废柴QWQ





## 列表

* \*
* \-
* \+
* 回车加tab，可以建立次级列表





## 区块

* Markdown 区块引用是在段落开头使用 **>** 符号 ，然后后面紧跟一个空格符号
* 区块是可以嵌套的，一个 **>** 符号是最外层，两个 **>** 符号是第一层嵌套，以此类推

### 区块的一些使用

* > 区块引用
  > 生活不易
  > 废柴努力
  
* > 最外层
  > > 第一层嵌套
  > >
  > > > 第二层嵌套
  
* > 区块中使用列表
  > 1. 第一项
  > 2. 第二项
  > + 第一项
  > + 第二项
  > + 第三项

* * 第一项
      > 生活不易
      > 废柴努力
  * 第二项





## 代码

* 单条语句
  * 使用反引号**`**把它包起来

* 代码区块
  * 使用四个空格或者一个制表符（Tab键）
  * 使用三个反引号**```**把它包起来

### 示例

`print("Hello World!")`

	#include<iostream>
	using namespace std;
	int main()
	{
		cout<<"Hello World!";
		return 0;
	}
```C
#include<stdio.h>
void main()
{
	printf("Hello World!");
}
```





## 链接

* 使用方式

  * [连接名称](链接地址)

  * <链接地址，例如 https://www.baidu.com>



* 高级用法

```
这个链接用 Google 作为网址变量 [Google][Google]
然后在文档的结尾为变量赋值（网址）

  [Google]: http://www.google.com/
```



## 图片

* 使用方式

* ```
  ![alt 属性文本](图片地址)
  
  ![alt 属性文本](图片地址 "可选标题")
  ```
  * 开头一个感叹号 !
  * 接着一个方括号，里面放上图片的替代文字
  * 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。

* 可以像网址那样对图片网址使用变量

* Markdown 还没有办法指定图片的高度与宽度，如果你需要的话，你可以使用普通的 <img> 标签

* ```
  <img src="图片地址" width="50%">
  ```





## 表格

Markdown 制作表格使用 **|** 来分隔不同的单元格，使用 **-** 来分隔表头和其他行。

语法格式如下：

```
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
```

* 对齐方式

  **我们可以设置表格的对齐方式：**

  - **-:** 设置内容和标题栏居右对齐。

  - **:-** 设置内容和标题栏居左对齐。

  - **:-:** 设置内容和标题栏居中对齐。

    - ```
      | 左对齐 | 右对齐 | 居中对齐 |
      | :-----| ----: | :----:|
      | 单元格 | 单元格 | 单元格 |
      | 单元格 | 单元格 | 单元格 |
      ```





## 高级技巧

* 支持的 HTML 元素

  * 目前支持的 HTML 元素有：`<kbd> <b> <i> <em> <sup> <sub> <br>`等

* 转义字符

  * Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符

  * Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号

  * ```
    \   反斜线
    `   反引号
    *   星号
    _   下划线
    {}  花括号
    []  方括号
    ()  小括号
    #   井字号
    +   加号
    -   减号
    .   英文句点
    !   感叹号
    ```

* 公式

  * 当你需要在编辑器中插入数学公式时，可以使用两个美元符 $$ 包裹 TeX 或 LaTeX 格式的数学公式来实现。提交后，问答和文章页会根据需要加载 Mathjax 对数学公式进行渲染

  * ```
    $$
    \mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
    \mathbf{i} & \mathbf{j} & \mathbf{k} \\
    \frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
    \frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
    \end{vmatrix}
    ${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
    $$
    ```

  * $$
    \mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
    \mathbf{i} & \mathbf{j} & \mathbf{k} \\
    \frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
    \frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
    \end{vmatrix}
    ${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
    $$

* 绘图（流程图、时序图(顺序图)、甘特图）

  * **1、横向流程图源码格式：**

    ```
    ​```mermaid
    graph LR
    A[方形] -->B(圆角)
        B --> C{条件a}
        C -->|a=1| D[结果1]
        C -->|a=2| E[结果2]
        F[横向流程图]
    ​```
    ```

  * ```mermaid
    graph LR
    A[方形] -->B(圆角)
        B --> C{条件a}
        C -->|a=1| D[结果1]
        C -->|a=2| E[结果2]
        F[横向流程图]
    ```

  * **2、竖向流程图源码格式：**

    ```
    ​```mermaid
    graph TD
    A[方形] --> B(圆角)
        B --> C{条件a}
        C --> |a=1| D[结果1]
        C --> |a=2| E[结果2]
        F[竖向流程图]
    ​```
    ```

  * ```mermaid
    graph TD
    A[方形] --> B(圆角)
        B --> C{条件a}
        C --> |a=1| D[结果1]
        C --> |a=2| E[结果2]
        F[竖向流程图]
    ```

  * **3、标准流程图源码格式：**

    ```
    ​```flow
    st=>start: 开始框
    op=>operation: 处理框
    cond=>condition: 判断框(是或否?)
    sub1=>subroutine: 子流程
    io=>inputoutput: 输入输出框
    e=>end: 结束框
    st->op->cond
    cond(yes)->io->e
    cond(no)->sub1(right)->op
    ​```
    ```

  * ```flow
    st=>start: 开始框
    op=>operation: 处理框
    cond=>condition: 判断框(是或否?)
    sub1=>subroutine: 子流程
    io=>inputoutput: 输入输出框
    e=>end: 结束框
    st->op->cond
    cond(yes)->io->e
    cond(no)->sub1(right)->op
    ```

  * **4、标准流程图源码格式（横向）：**

    ```
    ​```flow
    st=>start: 开始框
    op=>operation: 处理框
    cond=>condition: 判断框(是或否?)
    sub1=>subroutine: 子流程
    io=>inputoutput: 输入输出框
    e=>end: 结束框
    st(right)->op(right)->cond
    cond(yes)->io(bottom)->e
    cond(no)->sub1(right)->op
    ​```
    ```

  * ```flow
    st=>start: 开始框
    op=>operation: 处理框
    cond=>condition: 判断框(是或否?)
    sub1=>subroutine: 子流程
    io=>inputoutput: 输入输出框
    e=>end: 结束框
    st(right)->op(right)->cond
    cond(yes)->io(bottom)->e
    cond(no)->sub1(right)->op
    ```

  * **5、UML时序图源码样例：**

    ```
    ​```sequence
    对象A->对象B: 对象B你好吗?（请求）
    Note right of 对象B: 对象B的描述
    Note left of 对象A: 对象A的描述(提示)
    对象B-->对象A: 我很好(响应)
    对象A->对象B: 你真的好吗？
    ​```
    ```

  * ```sequence
    对象A->对象B: 对象B你好吗?（请求）
    Note right of 对象B: 对象B的描述
    Note left of 对象A: 对象A的描述(提示)
    对象B-->对象A: 我很好(响应)
    对象A->对象B: 你真的好吗？
    ```

  * **6、UML时序图源码复杂样例：**

    ```
    ​```sequence
    Title: 标题：复杂使用
    对象A->对象B: 对象B你好吗?（请求）
    Note right of 对象B: 对象B的描述
    Note left of 对象A: 对象A的描述(提示)
    对象B-->对象A: 我很好(响应)
    对象B->小三: 你好吗
    小三-->>对象A: 对象B找我了
    对象A->对象B: 你真的好吗？
    Note over 小三,对象B: 我们是朋友
    participant C
    Note right of C: 没人陪我玩
    ​```
    ```

  * ```sequence
    Title: 标题：复杂使用
    对象A->对象B: 对象B你好吗?（请求）
    Note right of 对象B: 对象B的描述
    Note left of 对象A: 对象A的描述(提示)
    对象B-->对象A: 我很好(响应)
    对象B->小三: 你好吗
    小三-->>对象A: 对象B找我了
    对象A->对象B: 你真的好吗？
    Note over 小三,对象B: 我们是朋友
    participant C
    Note right of C: 没人陪我玩
    ```

  * **7、UML标准时序图样例：**

    ```
    ​```mermaid
    %% 时序图例子,-> 直线，-->虚线，->>实线箭头
      sequenceDiagram
        participant 张三
        participant 李四
        张三->王五: 王五你好吗？
        loop 健康检查
            王五->王五: 与疾病战斗
        end
        Note right of 王五: 合理 食物 <br/>看医生...
        李四-->>张三: 很好!
        王五->李四: 你怎么样?
        李四-->王五: 很好!
    ​```
    ```

  * ```mermaid
    %% 时序图例子,-> 直线，-->虚线，->>实线箭头
      sequenceDiagram
        participant 张三
        participant 李四
        张三->王五: 王五你好吗？
        loop 健康检查
            王五->王五: 与疾病战斗
        end
        Note right of 王五: 合理 食物 <br/>看医生...
        李四-->>张三: 很好!
        王五->李四: 你怎么样?
        李四-->王五: 很好!
    ```

  * **8、甘特图样例：**

    ```
    ​```mermaid
    %% 语法示例
            gantt
            dateFormat  YYYY-MM-DD
            title 软件开发甘特图
            section 设计
            需求                      :done,    des1, 2014-01-06,2014-01-08
            原型                      :active,  des2, 2014-01-09, 3d
            UI设计                     :         des3, after des2, 5d
        未来任务                     :         des4, after des3, 5d
            section 开发
            学习准备理解需求                      :crit, done, 2014-01-06,24h
            设计框架                             :crit, done, after des2, 2d
            开发                                 :crit, active, 3d
            未来任务                              :crit, 5d
            耍                                   :2d
            section 测试
            功能测试                              :active, a1, after des3, 3d
            压力测试                               :after a1  , 20h
            测试报告                               : 48h
    ​```
    ```

  * ```mermaid
    %% 语法示例
            gantt
            dateFormat  YYYY-MM-DD
            title 软件开发甘特图
            section 设计
            需求                      :done,    des1, 2014-01-06,2014-01-08
            原型                      :active,  des2, 2014-01-09, 3d
            UI设计                     :         des3, after des2, 5d
        未来任务                     :         des4, after des3, 5d
            section 开发
            学习准备理解需求                      :crit, done, 2014-01-06,24h
            设计框架                             :crit, done, after des2, 2d
            开发                                 :crit, active, 3d
            未来任务                              :crit, 5d
            耍                                   :2d
            section 测试
            功能测试                              :active, a1, after des3, 3d
            压力测试                               :after a1  , 20h
            测试报告                               : 48h
    ```
