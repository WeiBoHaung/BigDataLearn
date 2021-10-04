# Day2 10/01 Python 程式語言基礎
###### tags: `大數據` `Python`


## 課程介紹

1. 課程名稱 : Python
2. 課程時數 :  小時
3. 使用軟體 : Anaconda
4. 書籍資料 : 
## 程式語言介紹
* 第一門課 - 程式語言的挑選 [影片連結](https://www.youtube.com/watch?v=BHFxFI5dhYE)
    ![](https://i.imgur.com/5WdOZLW.png)
* 第二門課 - 寫程式前的7分鐘重要觀念 [影片連結](https://www.youtube.com/watch?v=0iuJX47OsFo)
    ![](https://i.imgur.com/ujUhVgl.png)
    
    
## 操作環境設置
* 可選擇的開發用程式:
        * Anaconda
        * VisualStudio Code
        * VisualStudio 2019
* 系統需求:
        * 需要64位元

    ![](https://i.imgur.com/YPeZxL9.png)
    
* 安裝Anaconda，到[https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual)，下載

    ![](https://i.imgur.com/4pQNaQT.png)
* 記得安裝時這兩個需要勾選
![](https://i.imgur.com/ftgWU5H.png)

## 操作環境介紹

![](https://i.imgur.com/QEBuxAq.jpg)
![](https://i.imgur.com/1Q8rRCL.png)
![](https://i.imgur.com/z7b59nc.jpg)
![](https://i.imgur.com/i9uo6Pe.jpg)


## 語法介紹

![](https://i.imgur.com/aOGzLO8.png)

![](https://i.imgur.com/fYVG5xt.png)


### 變數

* = 的語法 : A=7意思是將7寫入名子叫A的記憶體，A=B+C意思是將B+C後寫入A，=的前面是變數，可議自行命名，需要英文開頭。
    ex :        ![](https://i.imgur.com/f6DCPyy.png)
    


        
    *    匈牙利命名法（Hungarian notation）是電腦程式設計中的一種變數命名規則。在匈牙利命名法中，一個變數名由一個或多個小寫字母開始，這些字母有助於記憶變數的類型和用途，緊跟著的就是程式設計師選擇的任何名稱。這個後半部分的首字母可以大寫，以區別前面的類型指示字母。
            * lAccountNum
            * arru8NumberList
            * szName

### Python基本資料型態

- 數值型態（Numeric type） - `int`, `float`, `bool`, `complex`
- 字串型態（String type）- `str`
- 容器型態（Container type） - `list`, `set`, `dict`, `tuple`

1. 整數 integer( int ) : 我們在上一段變數介紹的部分中，曾經產生過一個變數 a=7，  就是一個整數( integer)型態的變數。
    
    * 舉例:
        ```
        a = 1
        print(a)  #把a內容印出來
        print(type(a))   #把的型態印出來
        ```
    * 結果:
        ```
        1
        <class 'int'>
        ```
1. 浮點數 floating-point (float) : 上面產生了整數 a = 1 ，如果把他改寫成 a = 1.5 ，此時 a 就不是整數了，而是一種浮點數( float )。
    
    * 舉例:
        ```
        a = 1.5
        print(a)  #把a內容印出來
        print(type(a))   #把a的型態印出來
        ```
    * 結果:
        ```
        1.5
        <class 'float'>
        ```
1. 字串 string (str) : 字串資料是以單引號 (')或雙引號(")所包起來的文字資料，由一連串字元所組成。例如：
    
    * 舉例:
        ```
        song = "Hello, Goodbye0987654321"
        print(song)
        print(type(song))
        ```
    * 結果:
        ```
        Hello, Goodbye0987654321
        <class 'str'>
        ```
### 算術運算子

* 常用運算子

| 運算子 | 功能  | 範例 |
| - | - | --- |
| +     | 加     | a + b     |
| -     | 減     | a - b     |
| *     | 乘     | a * b     |
| **    | 指數    | a ** b     |
| /     | 除     | a / b     |
| //    | 整數除法    | a // b     |
| %     | 取餘數  | a % b     |


* 整除、取餘數:
```
3/2=1.5 (整數中，3 除 2 除不盡，商 : 1，餘 : 1)
a=3//2
b=3%2

a為1
b為1
```

* 舉例:
```
print(1 + 2)
print(1 - 2)
print(1 * 2)
print(2 ** 3)
print(4**(1/2)) #開二次方根
print(8**(1/3)) #開三次方根
print(1 / 2)
print(1 // 2)   #取商數
print(1 % 2)    ＃取餘數
```
 
* 會輸出：

```
3
-1
2
8
2
2
0.5
0
1
```

### 比較運算子

| 比較運算子 | 說明                   |
| ---------- | ---------------------- |
| >          | 大於                   |
| >=         | 大於或等於             |
| <          | 小於                   |
| <=         | 小於或等於             |
| ==         | 等於                   |
| !=         | 不等於                 |
| <>         | 不等於（與!=功能相同） |
* 舉例:
```
print('AAC' < 'ABC')
print([2, 3] > [4, 5])
print((2, 3) == (4, 5))
print({2, 3} > {4, 5})
print({'A': 3} == {'A': 3)
```

* 會輸出：

```
True
False
False
False
True
```

### 條件判斷

現實世界中總是充滿各種突發的狀況，程式的一些條件判斷與動作執行可以用來處理生活中所遇上的問題，讓程式的執行能夠因情況而轉彎。 例如：「當室內溫度超過 28 度時，就啟動冷氣運作。」、「當感測器所偵測的數值大於 60 時，就點亮紅色警示燈，否則點亮綠色警示燈。」

*  if-else敘述if 敘述還可以搭配 else 來使用，讓程式在 if 條件不成立時，便去執行 else 底下所定義的動作；也就是當判斷條件成立時做某事，判斷條件不成立時就做另外一件事。其語法如下：
    * 舉例:
        ```
        score = 50
        if score >=70:
            print('及格')
        else:
            print('分數不及格')
        ```
    * 輸出結果:
        ```
        分數不及格
        ```
    


### print 輸出
在 Python 中，我們常常會需要將既有的數值輸出到電腦螢幕上，以便程式的測試等工作。這種時候，print() 函數就可以發揮它無比強大的功用。

* 舉例:
    ```
    a = 3
    print(a)
    ```
* 輸出結果:
    ```
    3
    ```

print() 函數還有很多有趣的地方。現在先讓我們建立兩個變數，一個叫做 a，另一個叫做 b，分別代表 Hello 與 World，在 print() 函數中，用逗號將要印出的東西分開，Python 將會自動將各個變數連結起來並印出：
* 舉例:
    ```
    a = "Hello"
    b = "World"
    print(a, b)
    ```
* 輸出結果:
    ```
    Hello World
    ```

### input 輸入

有時候，我們除了輸出之外，也會想要從使用者那邊得到輸入的值。在 Python 中，獲得使用者輸入的值是相當簡單的。讓我們來看看以下的例子：
* 舉例:
    ```
    a = input()
    ```
* 輸出結果:
    ```
       <<_     #執行後停住，等待使用者輸入
       
       test input data #這是我們使用者輸入的字 然後敲enter
       test input data #這時程式就會輸出我們使用者輸入的字
       
    ```

在這段程式的第一行中，我們先宣告了一個變數叫做 a，並且將其值設定為使用者所輸入的值。接著在第二行，使用者輸入了「Hi」，此時，a 的值被設定作「Hi」。第三行時，我們要求電腦印出 a 這個變數，因此電腦便在第四行的地方印出了「Hi」。

input() 的括號中，是可以放入參數的。放入的東西將會變成輸出字串，舉例來說：
* 舉例:
    ```
    a = input("Enter something: ")
    print(a)
    ```
* 輸出結果:
    ```
       <<Enter something: _     #執行後會出現Enter something: 後停住，等待使用者輸入
       
       test input data #這是我們使用者輸入的字 然後敲enter
       test input data #這時程式就會輸出我們使用者輸入的字
       
    ```
### 比較運算子

| 比較運算子 | 說明                   |
| ---------- | ---------------------- |
| >          | 大於                   |
| >=         | 大於或等於             |
| <          | 小於                   |
| <=         | 小於或等於             |
| ==         | 等於                   |
| !=         | 不等於                 |
| <>         | 不等於（與!=功能相同） |

* 舉例:

    ```
    x = [2, 3]
    y = [2, 3]
    print(x == y)
    print(x is y)
    ```

* 輸出結果:

    ```
    True
    False
    ```

除了數字之外，字串、`list`、`set`、'tuple'和`dict`也都可以進行比較運算，其運算依從第一個元素依照順序做比較，而字元的比較為比較其字元碼（如英文字為ASCII碼），例如：
* 舉例:

    ```
    print('AAC' < 'ABC')
    print([2, 3] > [4, 5])
    print((2, 3) == (4, 5))
    print({2, 3} > {4, 5})
    print({'A': 3} == {'A': 3)
    ```

* 輸出結果:

    ```
    True
    False
    False
    False
    True
    ```
    
    
### 課堂練習
結合上面介紹功能，寫一個輸入分數，回傳對應評語

```
score = int(input("輸入分數"))
if score <50:
    print("再見")
elif score <60:
    print("補考")
elif score <70:
    print("普通")
elif score <80:
    print("很好")
else:
    print("非常好")
```
也可以這樣寫
```
score = int(input("輸入分數："))
if score >=80:
    print("非常好")
elif score >=70:
    print("很好")
elif score >=60:
    print("普通")
elif score >=50:
    print("補考")
else:
    print("再見")
```
大到小
```
score=int(input("輸入分數："))
if score>79:
    print("非常好")
elif score>69:
    print("很好")
elif score>59:
    print("普通")
elif score>49:
    print("補考")
else:
    print("再見")
```