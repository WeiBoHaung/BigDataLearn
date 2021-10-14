# Day8 10/12  機器學習資料分析實務
###### tags: `大數據` 

* 今日目標 : 寫出可機器學習的程式。
* 機翼學習 : 用程式語言模擬出大腦神經元的反應。
* soma : 腦神經元輸入端
* dendrites : 腦神經元輸出端
* axon:主神經線 輸出（電脈衝*1）
* synapse:微量化學物質 輸入（量）
* perceptron:單一神經細胞感知器（模擬大腦其一）
* activation function: 受刺激（激活）的反應方程式 
    1. Step function
    2. Sign function
    3. Sigmoid function 
    4. Linear function





## 機器學習方法
### 神經元反應 舉例
![](https://i.imgur.com/jcRMkHZ.png)

* Activation function 神經元以激活函式表示如下:（受刺激後之反應方程式，主要目的為計算$Y_a$真實反應值）
     $X=\sum_{i=1}^{n}x_iw_i$ ,

     $Y=\left\{ \begin{array}{ll}
        +1,if \quad X\geq \theta\\
        -1,if \quad X<\theta
        \end{array} \right.$
### or/and學習的演算法 
* $w_i(p+1)=w_i(p)+\alpha \cdot x_i(p)\cdot e(p)$
    * $w_i$ : 神經節點
    * $p$ : 這一次
    * $p+1$ : 下一次
    * $x_i$ : 輸入值，0或是1
    * $e$ : 誤差值 $e=Y_d-Y_a$
    * $\alpha$ : 放大倍數，這裡預設0.2

* Step 1: Initialisation
    設定參數，e、X1、X2、Yd、Ya
* Step 2: Activation
    輸入數值 $x_1(p)$, $x_2(p)$… $x_n(p)$ ，n是感知器數量，帶入以下
    
    * If x1*w1+x2*w2>$\Theta$ :
        * $Y_a=1$
    * else: 
        * $Y_a=0$
    * 計算誤差值 $e=Y_d-Y_a$
* Step 3: Weight training
    如果誤差$e$不等於0，則執行以下調整$w_i$
    * $w_i(p+1)=w_i(p)+\alpha \cdot x_i(p)\cdot e(p)$
    
* Step 4: Iteration
    反覆執行2、3步驟職到所有答案符合期望值。

## 課堂練習
### 寫出Perceptron Learning進行and/or學習時全部演算法
* 題目 :
    ![](https://i.imgur.com/8K4kjn8.png)
* 解答 : 
    ![](https://i.imgur.com/ioDpOHc.gif)
    > [name=Web_Haung]
* 程式碼 : 
```
import numpy as np

def getYa(x1,x2,w1,w2,Theta):
    if x1*w1+x2*w2>Theta:
        print(x1,'X',w1,'+',x2,'X',w2,'>',Theta,'Ya=1')
        return 1
    else: 
        print(x1,'X',w1,'+',x2,'X',w2,'<=',Theta,'Ya=0')
        return 0
def gete(yd,ya):
    return np.round( yd-ya)

if __name__ == '__main__':
    w1=np.round( float(input('w1:')),4)
    w2=np.round( float(input('w2:')),4)
    Theta=np.round( float(input('Theta:')),4)
    yd=input('輸入Yd :')
    yd=[int(n) for n in yd.split()]
    index=0
    check_count=1
    while 1:
        print('-------------------------')
        if index==4:
            index=0
        x1=np.round( float(input('x1:')),4)
        x2=np.round( float(input('x2:')),4)
        ya=getYa(x1,x2,w1,w2,Theta)
        e=gete(yd[index],ya)
        # index=index+1
        print('目前Yd :',yd[index],'，Ya :',ya,'e=Yd-Ya')

        if e!=0:
            w1=np.round(w1+0.2*x1*e,4)
            w2=np.round(w2+0.2*x2*e,4)
            check_count=0
            print('誤差',e,'，修正')
        else:
            print('誤差0，不修正')
            check_count=check_count+1
            index=index+1
    
        print('w1 : ',w1,'/w2 : ',w2)
        if check_count==4:
            print('-----------答--------------')
            print('  w1 : ',w1,'/w2 : ',w2)
            break
    
```
## 截圖區
![](https://i.imgur.com/AGE1ekH.png)

![](https://i.imgur.com/2kCXhY6.png)

![](https://i.imgur.com/itJCYBo.png)

![](https://i.imgur.com/ax2TOfN.png)

![](https://i.imgur.com/qpdgtqU.png)

1. ![](https://i.imgur.com/9KK9i3e.png)

1. ![](https://i.imgur.com/HEItasX.png)

1. ![](https://i.imgur.com/T5zKFOT.png)

1. ![](https://i.imgur.com/avKijoL.png)

1.![](https://i.imgur.com/wzrJKON.jpg)





1. ![](https://i.imgur.com/Hx4fVA5.png)

1. ![](https://i.imgur.com/oa3YoTp.png)

1. ![](https://i.imgur.com/SxO6OtY.png)

1. ![](https://i.imgur.com/KY6ePW7.png)

1. ![](https://i.imgur.com/3rRg7Gz.png)

![](https://i.imgur.com/wnTyRCF.jpg)


![](https://i.imgur.com/0zScEK1.jpg)

![](https://i.imgur.com/puCvW9J.png)


![](https://i.imgur.com/ZvZp31O.jpg)

![](https://i.imgur.com/o2RCFGG.jpg)

![](https://i.imgur.com/B8WgOLp.png)


