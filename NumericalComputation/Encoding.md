# 1 of N Encoding 把单词转成向量

## 方法一：  

例如单词表为：lexicon = {apple, ball, cat}
那么这三个单词的向量依次为：  
apple = [1 0 0 0]  
ball = [0 1 0 0]  
cat = [0 0 1 0]
其它单词 = [0 0 0 1]  

## 方法二 word hashing：  

![](/assets/images/7.png)