# Day10 10/14  下午 Python 程式語言基礎
###### tags: `大數據` 

## threading 模組
### 描述
* threading 是 Python 標準函式庫裡面的模組，所以不用特別安裝即可使用，雖然功能不是很多，但是基本多執行緒程式設計常用的功能它都有，用來撰寫多執行緒（multithreading）的平行化程式。

* 程式碼
    ```python
    import threading
    import time

    class myClass(threading.Thread):#繼承
        def __init__(self, x):
            threading.Thread.__init__(self)
            self.y = x
        def run(self):
            for i in range(3):
                print (self.y,'說話')

    myClass('A').start()
    myClass('B').start()
    myClass('C').start()
    myClass('D').start()
    ```
* 運作過程
    * 無多執行緒，會看到A說完話才會輪下一個:
    ![](https://i.imgur.com/XkSPXxD.gif)

    * 有多執行序，會看到同時好幾個說話:
    ![](https://i.imgur.com/uHDqMwm.gif)

