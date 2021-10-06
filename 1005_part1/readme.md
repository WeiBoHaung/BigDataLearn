# Day4 10/05 上午 Python 程式語言基礎
###### tags: `大數據` `Python`


## if
```
if 條件1:
    做1的事情
elif 條件2 :
    做2的事情
elif 條件3 :
    做3的事情
else:
    否則做這些事
```

## 課堂練習
一年有12個月，問→輸入月，回傳天數。
1. 需檢查輸入是否超出月份是否吃出範圍。
2. 輸入錯誤的時候，要回傳錯誤訊息。

```
x=int(input('輸入月份'))

if x<1 or x>12 :
    print('輸入錯誤數字')
elif x>0 and x<8 and x%2==1:
    print('31天')
elif x>7 and x<13 and x%2==0:
    print('31天')
elif x>7 and x<13 and x%2==1:
    print('30天')
elif x==2:
    print('28天')
else:
    print('30天')

```
BMI 很重要吧！衡量體重的一個重要指標，然而有時要計算一堆個案需要達到多少體重才符合標準也挺麻煩的，所以用 Python 寫一個小程式，可以計算BMI並分類，再計算出體重需要達到多少才符合正常體位。
* BMI = weight(kg) / height(m)2
```
#使用者輸入資訊
weight = int(input("體重(kg): "))
height = int(input("身高(cm): "))

#身高公分轉公尺
height = height / 100

#BMI 計算，四捨五入小數第二位
BMI = round(weight / (height ** 2),2)
print("\nBMI 計算結果 = " + str(BMI))
if BMI < 18.5:
    print( "BMI 過低，體重過輕")
elif BMI<24:
    print( "BMI 正常，標準體位")
else:
    if BMI < 27:
        print( "BMI 過高，體重過重")
    elif BMI < 30:
        print( "BMI 過高，輕度肥胖")
    elif BMI < 35:
        print( "BMI 過高，中度肥胖")
    else:
        print( "BMI 過高，重度肥胖")


```
##  for 迴圈

### 語法

for i in 一個區間:
    print(i)
    
* 舉例
    ```
    print('程式開始')
    index=1
    for i in [1,2,'a','b','k',9,3,2]:
        print('目前是第',index,'圈，i目前跑到的內容是',i)
        index=index+1
    print('程式結束')
    ```
* 輸出效果
    ![](https://i.imgur.com/46E90PF.png)
