# Day5 10/06 Python 程式語言基礎
###### tags: `大數據` 

## 課堂練習
### 小數轉整數-小數點後取三位，無條件捨去
* 程式碼
    ```
    x=23.1234
    print( int(x*1000))
    ```
* 輸出結果
    ![](https://i.imgur.com/mhTfKkK.png)
  
### 四捨五入，小數點後一位

* 老師程式碼
    ```
    p=1 #精確度 取小數點後幾位
    if p>0:
        x=23.2176
        x=x*(10**(p+1))
        if x%10<=4:
            x=int(x-x%10)/(10**(p+1))
        else:
            x=int(x-x%10)/(10**(p+1))+1/(10**9)
    elif p==0:
        pass
    else:
        pass
    print(x)
    ```
    
* 同學程式碼
    ```
    x=23.2176
    if x%100 <5 :
        print( int(x*10)/10)
    else:
        print( int(x*10+1)/10)
    ```
* 輸出結果
   ![](https://i.imgur.com/x5yHC9C.png)
   
## 型態介紹
### list
* 介紹:
    序列是Python中最基本的數據結構。序列中的每個元素都分配一個數字 - 它的位置，或索引，第一個索引是0，第二個索引是1，依此類推。
* 舉例:
    ```
    list1 = ['physics', 'chemistry', 1997, 2000]
    list2 = [1, 2, 3, 4, 5 ]
    list3 = ["a", "b", "c", "d"]
    ```   
### float
* 介紹:



## 語法介紹 

### range
* 語法介紹: 
    `range(開始, 結束,間隔])`
* 舉例:
    ![](https://i.imgur.com/X5STDWu.gif)
    ![](https://i.imgur.com/8XE9yhM.gif)


### import
* 語法介紹: 
    `import 模組名稱 as 簡稱`
* 舉例:
    ```
    import Math as Ma
    
    ```
* 注意事項:
    ![](https://i.imgur.com/Mxdvp1n.png)
    ![](https://i.imgur.com/lBEz09O.gif)



    使用的時候，必須要掛上模組名稱，原因是?有可能不同的模組，有相同的名稱的處理方法。
    以上圖為例如果只用top()，python會無法分變你要使用哪個模組的top()方法。

### random

* 描述
    random() 方法返回随机生成的一个实数，它在0~1范围内。

* 舉例:
    ```
    import random #記得要import
    
    print( random.randint(1,10) )        
    # 产生 1 到 10 的一个整数型随机数  
    
    print( random.random() )             
    # 产生 0 到 1 之间的随机浮点数
    
    print( random.uniform(1.1,5.4) )     
    # 产生  1.1 到 5.4 之间的随机浮点数，区间可以不是整数
    
    print( random.choice('tomorrow') )   
    # 从序列中随机选取一个元素
    
    print( random.randrange(1,100,2) )   
    # 生成从1到100的间隔为2的随机整数
    ```
    ![](https://i.imgur.com/aoC3HyZ.gif)
     
### break
* 描述:
    跳離整個迴圈。
* 舉例:
    ```
    print('開始')
    for i in range(10):
        if i ==5 :
            break
        print(i)

    print('結束')
    ```
    ![](https://i.imgur.com/WkNxFj8.gif)

### countinue
* 描述:
    跳離當下這一圈。
* 舉例:
    ```
    print('開始')
    for i in range(10):
        if i ==5 :
            countinue
        print(i)

    print('結束')
    ```
    ![](https://i.imgur.com/jxhUtA8.gif)



---
## 暫存截圖區
![](https://i.imgur.com/2KwaqqD.png)
     
![](https://i.imgur.com/jIDPQqI.png)

![](https://i.imgur.com/djZ3Q4Q.png)


![](https://i.imgur.com/8qYXwYa.png)
![](https://i.imgur.com/wCORug3.gif)
