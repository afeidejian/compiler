# 编译原理作业一
## 问答题
+ ### 编译系统通常由哪几个部分组成？简述各部分完成的功能。  

  * **编译系统由预处理器、编译器、汇编器、链接器和加载器组成**  

  * **预处理器**：负责把源程序聚合在一起，把宏转换为源程序  

  * **编译器**：将源程序输出为目标程序。从高级语言到低级语言  

  * **汇编器**：处理汇编语言程序，生成可重定位的机器代码  

  * **链接器**：负责解决不同文件代码链接时外部内存地址处理问题  

  * **加载器**：把所有可执行文件放到内存  

+ ### 编译器通常可以分成哪几个部分组成？每个部分的工作原理与实现的功能是什么？  

  + **词法分析器(lexical analysis)**：  
  
    * 读入组成源程序的字符流，组织称有意义的词素的序列，生成`<name,value>`的词法单元  
  + **语法分析器(syntax analysis)**：    
    * 将词法单元流生成对应的语法树(syntax tree)
  + **语义分析器(semantic analyzer)**：  
    * 使用语法树和语义表中的信息来检查源程序是否和语义定义的语义一致 搜集类型信息 检查类型
  + **中间代码生成器**：  
    * 生成一个明确的、低级的或类机器语言的中间表示   易于生成，且能轻松的翻译为目标机器上的语言
  + **机器无关代码优化器**：
    * 代码优化
  + **代码生成器**：
    * 将源程序的中间表示形式映射到目标语言，分配寄存器或内存来存放变量
  + **机器相关代码优化器**：
    * 代码优化


## 思考题 
+ ### 词法分析的原理是什么？如何实现构词的？
+ ### 编译原理技术发展史




