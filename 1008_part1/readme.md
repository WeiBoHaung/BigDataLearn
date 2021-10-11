# Day6 10/08 早上  Python 程式語言基礎
###### tags: `大數據` `PowerBI`



## dictionary 型態
* 敘述 :
    每一個元素都由鍵 (key) 和值 (value) 構成，結構為key: value 。不同的元素之間會以逗號分隔，並且以大括號 {}圍住。
* 語法 :
    `xxx = {key1: value1, key2: value2}`
* 範例程式碼 :
    ```
    movie = {'name':'Saving Private Ryan', #電影名稱
                'year':1998, #電影上映年份
                'director':'Steven Spielberg',#導演
                'Writer': 'Robert Rodat', #編劇
                'Stars':['Tom Hanks', 'Matt Damon', 'Tom Sizemore'],#明星
            }
    print('電影名稱 : ',movie['name'])
    print('電影上映年份 : ',movie['year'])
    print('導演 : ',movie['director'])
    print('編劇 : ',movie['Writer'])
    print('明星 : ',movie['Stars'][0],'、',movie['Stars'][1],'、',movie['Stars'][2])
    ```
* 輸出結果 :
    ![](https://i.imgur.com/6gF0qQh.png)

## tuple
* 敘述 :
    tuple 是 Python 的資料儲存容器之一，最大的特點就是，它是「不可變」（Immutable）的資料型態。
    1. 因為不可變（immutable）的特性，運作起來比串列還要快。
    1. 不會不小心改變 tuple 的值，也就是 tuple 的項目不會不小心被更動到。
    1. 占用的空間比較少。
    1. 作為字典（dictionary）的鍵（key）使用，因為字典的鍵需要不可變的值。
    1. 具名 tuple 可以簡易的作為物件的替代品。

* 語法 :
    `number = (1, 2, 3)`
* 範例程式碼 :
    ```
    number = (1, 2, 3)
    print('number的內容 : ',number,'\nnumber的型態 : ',type(number))
    ```
    
* 輸出結果 :
    ![](https://i.imgur.com/3I9nEru.png)
    
* 注意tuple 與list主要有三點不同 : 
    1. 使用的符號不同
        tuple ，用小括號表示 。
        例如 (‘a’, ‘b’)。

        list，用中括號表示 。
        例如 [‘a’, ‘b’]。
        
    1. tuple屬於不可變的資料型態
        不可變（Immutable）是什麼意思？就是你不可以修改、增減tuple的值。
        也因為 tuple 不可變的特性，所以沒有append()、remove()、pop()等會更動值的操作。
        
    1. 只含有一個項目時，要加上逗點
        當你要建立只有一個項目的 tuple，千萬要記得加上逗號，否則不會建立 tuple。
## 函數介紹
### enumerate
* 敘述 :
    enumerate() 函數用於將一個可遍歷的數據對象(如列表、元組或字符串)組合為一個索引序列，同時列出數據和數據下標，一般用在 for 循環當中。
    
* 語法 :
    `enumerate(iterable, start=0)`
* 範例程式碼 :
    ```
    Fruits = ['Apple', 'Mango', 'Orange']
    print('單輸出內容 : ')
    for item in enumerate(Fruits):
      print(item)

    print('\n輸出內容+index : ')
    for count, item in enumerate(Fruits):
      print(count, item)

    print('\n輸出內容+index，改變index起始編號 : ')
    for count, item in enumerate(Fruits, 50):
      print(count, item)
    ```
    
* 輸出結果 :
![](https://i.imgur.com/faJfTiy.png)

## 自訂涵式
首先給函數取個名字（function_name），接著在小括號中放進輸入（inputs）與參數（parameters），然後附上一段說明（Docstrings），在縮排內撰寫我們主要的程式，最後把輸出結果放在 return 後面。

* Python 自訂函數的架構：

```
def function_name(輸入1, 輸入2, 參數 1, 參數 2, ...):
    """
    Docstrings
    """
    # 主要的程式
    return 結果
```