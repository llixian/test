# test
##功能：  
1.题目避免重复。  
2.判定用户输入的答案是否正确。  
3.可以控制下列参数：  
是否有乘除法  
是否有括号  
参与运算的数值范围  
加减有无负数  
乘除有无余数  
4.处理四种运算的混合算式。 ##代码实现： 使用c++实现，用户可以选择是否有括号，乘除法等。 首先还是生成一道两个数的四则运算式，多个数的运算只是在两个数的基础上进行增加的，所以可以把上一次生成的运算式当作一个数，再与随机生成的另一个数合成一个运算式，如此循环，直到整个运算式的数字个数满足我想要达到的数量为止。 字符串有的合成可以直接把几个字符串相加，于是可以把每一次生成的运算式转换成字符串的形式来存放，这个过程中要使用到itoa()函数。这样的话如果要加入“（）”也会变得非常简单，判断题目是否有重复，只需把每次新生成的运算式存放在字符串数组中，依次比较之前生成的运算式中是否有相同项，若有，则此次生成无效，再重新生成一个新的运算式，若没有重复项，则进行下一道运算式的生成工作。直到达到生成运算式的数量为止。 最后，用到数据结构中的栈来解决表达式的求值，判断正误。    
##界面展示  
![image](https://github.com/llixian/test/blob/master/images/2.PNG)  
![image](https://github.com/llixian/test/blob/master/images/3.PNG)  
![image](https://github.com/llixian/test/blob/master/images/4.PNG)  
