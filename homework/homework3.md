# 编译原理作业三
## 1.描述下列正规式（正则）定义的语言（请用汉语直白地描述该语言）
#### a) 0(0 | 1)*0  

长度大于等于2 开头结尾为0的 由0和1组成的字符串

#### b) ((e | 0)1*)*  
任意由由0和1组成的字符串 包括空

#### c) (0|1)*0(0|1)(0|1)  
长度大于等于3 左数第三位为0的 由0和1组成的字符串

#### d) 0*10*10*10*  
只含有3个1的 由0和1组成的字符串

#### e) (00 | 11)\*((01 | 10)(00 | 11)\*(01 | 10)(00 | 11)\*)\*   
偶数个0偶数个1构成的字符串 可为空

## 2. 为下列语言写出正规定义(或正规式、正规文法、有限自动机) 


#### a) 包含五个元音，且按顺序排列的所有字母串（RE） 

设S=(b|c|d|f......|t|v|w|x|y|z) 即不含元音  
S\*a(a|S)\*e(e|S)\*i(i|S)\*o(o|S)\*u(u|S)\*


#### b) 字母按字典升序排列的所有字母串（RE）
A\*B\*C\*....X\*Y\*Z\*a\*b\*c\*d\*........x\*y\*z\*  共52个

#### c)以/\*开始，\*/结束的注释，中间不能包含\*/，除非包含在"和"中（RE）
(\\/\\\*)([^\*"]\*|".\*"|\\\*+[^/])*(\\\*\\/)


![Image text](https://github.com/YULuoOo/compiler/blob/master/homework/QQ20190312-0.png)


#### d) 不包含重复数字的数字串（DFA）


#### e) 包含至多一个重复数字的数字串（DFA）


#### f) 包含偶数个0和奇数个1的0、1串 (DFA)