# Day13 10/19 下午 機器學習資料分析實務
###### tags: `大數據`

## 使用 $x_1w_1+x_2w_2-\theta=0$ 做 xor學習探討
![](https://i.imgur.com/ILdOROc.gif)
* 會發現$w_1$、$w_2$會一直$++--$無法收斂。
## 檢視反映方程式 $x_1w_1+x_2w_2-\theta=0$
### $x_1w_1+x_2w_2-\theta=0$其實就是幾何代數的$ax+by-c=0$的直線方程式。
* 此直線方程式解釋如下:
    * $ax+by-c=0$
        * a、b視為係數(決定直線的斜率)
        * c 為截距
    * $x_1w_1+x_2w_2-\theta=0$
        * $w_1$、$w_2$視為係數(決定直線的斜率)
        * $\theta$ 為截距
* 反映方程式$x_1w_1+x_2w_2-\theta=0$其實就是平面上的一條線。
    * 當$w_1$、$w_2$、$\theta$的值已確定，就決定了該直線的位置。
    * 而>=0，代表輸入點的為ˋ在直線的上方或直線上

## 多層感知器
![](https://i.imgur.com/zU7QbaM.png)
![](https://i.imgur.com/zmufiGm.png)
## python 程式實做
### print練習
* 題目 :
    ![](https://i.imgur.com/FFPp7Fl.png)


* 程式碼 :
    ```python
    #雙回圈寫法
    def Righttriangle():
        for i in range(9):
            for k in range(i):
                print("★",end='')
            print("")

    def Invertedrighttriangle():
        for k in range(9,0,-1):
            for j in range(k):
                print("☆",end='')
            print("")

    def Christmastree():
        print("          ★")
        for a in range(10,0,-1):
            for b in range(a):
                print(" ",end='')
            for c in range(11-a):
                print("*",end='')
            for d in range(11-a):
                print("*",end='')
            print()  

    Righttriangle()
    Invertedrighttriangle()
    Christmastree()

    ```
    
* 輸出畫面 :
    ![](https://i.imgur.com/cIZ00h7.gif)

* 程式碼 :
    ```python
    #單迴圈
    for i in range(8):
        print("* " * i)
    for i in range(6,0,-1):
        print("* " * i)
    for i in range(11):
        print(" "*(10-i)+"* "*i)
    ```
    
* 輸出畫面 :
    ![](https://i.imgur.com/AfGU3D4.png)

## 截圖區
![](https://i.imgur.com/MUjvMvJ.png)
![](https://i.imgur.com/FSTRY8u.png)
![](https://i.imgur.com/7uqp46b.png)
![](https://i.imgur.com/cIMHz9G.png)

![](https://i.imgur.com/eRRArvC.png)
![](https://i.imgur.com/KRiUwBV.png)
![](https://i.imgur.com/zU7QbaM.png)
![](https://i.imgur.com/zmufiGm.png)

![](https://i.imgur.com/6yiDz1k.png)

![](https://i.imgur.com/13Sg7f7.png)

![](https://i.imgur.com/jvK9YAx.png)

![](https://i.imgur.com/abAsiJV.jpg)
![](https://i.imgur.com/mzVLsbC.png)
![](https://i.imgur.com/1pE8JCy.jpg)
![](https://i.imgur.com/ZGo6eJZ.png)


![](https://i.imgur.com/qvxyOwb.png)
![](https://i.imgur.com/LcaZJMY.jpg)
![](https://i.imgur.com/VeweXzD.png)
![](https://i.imgur.com/G8Mxt7m.png)
![](https://i.imgur.com/7dc2lkl.jpg)
![](https://i.imgur.com/GfGkdA6.png)

