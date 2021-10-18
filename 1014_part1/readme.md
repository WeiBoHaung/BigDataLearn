# Day10 10/14  上午 Python數據科學計算Numpy
###### tags: `大數據` 

## vsCode開Jupyter Notebooks檔
* 直接新建副檔名為ipynb的檔案，就會出了
    舉例 :
    ![](https://i.imgur.com/fhV2hiV.png)
    
* 新增ipynb的檔案的畫面
    ![](https://i.imgur.com/d8w8Hxq.png)

## 基礎操作
### array
* 敘述 : 
    * 一般我們稱一維陣列為 vector 而二維陣列為 matrix。一開始我們會引入 numpy 模組，透過傳入 list 到 numpy.array() 創建陣列。
* 結構 : 
    `numpy.array(object, dtype = None, copy = True, order = None, subok = False, ndmin = 0)`
    
    | 名稱 | 描述 |
    | -------- | -------- |
    |object|數組或嵌套的數列|
    |dtype|數組元素的數據類型，可選|
    |copy|對像是否需要復制，可選|
    |order|創建數組的樣式，C為行方向，F為列方向，A為任意方向（默認）|
    |subok|默認返回一個與基類類型一致的數組|
    |ndmin|指定生成數組的最小維度|


* 程式碼 : 
    ```python
    import numpy as np
    a=[1,3,5,7]
    print(a)
    print(type(a))
    print(type(a[0]))
    x1=np.array(a)
    print(x2)
    print((type(x2)))
    print(type(x2[0]))

    ```
* 輸出結果 : 
    ![](https://i.imgur.com/JpCPlsu.png)
    
### 数据类型对象 (dtype)

* 結構 : 
    `numpy.dtype(object, align, copy)`
    * object - 要轉換為的數據類型對象。
    * align - 如果為 true，填充字段使其類似 C 的結構體。
    * copy - 複製 dtype 對象 ，如果為 false，則是對內置數據類型對象的引用。
* 程式碼 : 
    ```python
    import numpy as np
    e = np.array([1,2.1,3,4,5], dtype=np.int8) 
    print('所有數字轉整數',e)
    ```
* 輸出結果 : 
    ![](https://i.imgur.com/sNbdbRa.png)



### arange

* 敘述 : 
    * 根據 start 與 stop 指定的範圍以及 step 設定的步長，生成一個 ndarray。
* 結構 : 
    `numpy.arange(start, stop, step, dtype)`
    | 名稱 | 描述 |
    | -------- | -------- |
    |start|起始值，默認為0|
    |stop|終止值（不包含）|
    |step|步長，默認為1|
    |dtype|返回ndarray的數據類型，如果沒有提供，則會使用輸入數據的類型。|
    

* 程式碼 : 

    ```python
    import numpy as np
    b = np.arange (0,10,1) 
    print ('印出np.arange (0,10,1) :  \n',b)
    c = np.arange (0.1, 10, 1.1)
    print ('印出np.arange (0.1,10,1.1) : \n',c)
    ```
    
* 輸出結果 : 
    ![](https://i.imgur.com/nMw1FeC.png)
    
### shape

* 敘述 : 
    * 是查看矩陣或者數組的維數。
* 結構 : 
    `numpy.shape` 
    
* 程式碼 : 

    ```python
    import numpy as np
    x=np.array([[ 1.,  0.,  0.],  
           [ 0.,  1.,  0.],  
           [ 0.,  0.,  1.]]) 
    print('x: \n',x,'\nx.shape : ',x.shape)
    ```
    
* 輸出結果 : 
    ![](https://i.imgur.com/GUHR3fV.png)


### linspace
* 敘述 : 
    * 用於創建一個一維數組，數組是一個等差數列構成的。
* 結構 : 
    `np.linspace(start, stop, num=50, endpoint=True, retstep=False, dtype=None)`
    | 名稱 | 描述 |
    | -------- | -------- |
	|start|序列的起始值|
	|stop|序列的終止值，如果endpoint為true，該值包含於數列中|
	|num|要生成的等步長的樣本數量，默認為50|
	|endpoint|該值為 true 時，數列中包含stop值，反之不包含，默認是True。|
	|retstep|如果為 True 時，生成的數組中會顯示間距，反之不顯示。|
	|dtype|ndarray 的數據類型|
* 程式碼 : 

    ```python
    import numpy as np
    f = np.linspace(0,10,11)
    print (f)
    ```
* 輸出結果 : 
    ![](https://i.imgur.com/ILBDrX0.png)


## 未整理
```
a=[1,3,5,7]
b=[2,4,6,8]
print(type(a))
print(type(a[0]))
c = a + b
print(c)
d = [x+y for x,y in zip(a,b)]
print(d)

import numpy as np
x1=np.array(a)
x2=np.array(b)
print(x2)
print((type(x2)))
x3=x1+x2
```