# Day6 10/07 下午 Python 程式語言基礎
###### tags: `大數據` `PowerBI`

## list
* 由來:
    假設一個學校6000人那就需要6000變數來裝每個人的資料嗎，那設計師就要一堆時間來新增這些資料了，太浪費時間了。
* 陣列特性包括：
    1. 可以儲存多個資料，就像建立一個資料清單，可以放入很多資料，相同的資料可以重複出現。
    2. 屬於序列結構，序列，指的是串列內的值有順序性，所以可以使用各種有關順序的方法 （Method） 進行操作；結構，指的是資料結構（data structure）是電腦中儲存、組織資料的方式。
    3. 值是可變的 （mutable），可以刪除、增加、修改串列的值，可以更動串列內的各個項目。

* 語法
    `[內容一,內容二,內容三]`
* 舉例:
    ```
    list1 = ['physics', 'chemistry', 1997, 2000]
    list2 = [1, 2, 3, 4, 5 ]
    list3 = ["a", "b", "c", "d"]
    print(list1[0]) #印出list1陣列的第一格內容
    print(list1[1])
    print(list1[2])
    ```   
### list相關函式
晚點補
## 語法介紹
### len()
* 描述:
    用來取得列長度。
* 語法介紹: 
    `len(陣列)`
* 舉例:
    ![](https://i.imgur.com/cTuJa7o.gif)
### 使用len+for迴圈逐一讀取
* 程式碼:
    ```
    index=0
    list = ["a", "b", "c", "d"]
    for i in range(len(list)):
        print('目前index=',index,'list目前讀取到',list[index])
        index=index+1
    ```
    ![](https://i.imgur.com/FeQKZYj.gif)
### 直接用for讀取陣列
* 程式碼:
    ```
    list1 = ["a", "b", "c", "d"]
    for i in list1:
        print('list目前讀取到',i)

    ```
    ![](https://i.imgur.com/BZwpBrE.gif)
### for len list練習
* 題目:
    設計一個陣列，將陣列裡低於60的改成不及格。
* 程式碼:
    ```
    score=[100,2,30,50,70,90]
    for i in range(len(score)):
        if score[i] < 60 :
            score[i]='不及格'

    for i in score:
        print(i)
    ```
    ![](https://i.imgur.com/a6WnjEj.gif)


## 暫存截圖區