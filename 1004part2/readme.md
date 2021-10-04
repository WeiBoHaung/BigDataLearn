# Day 3 下午 10/04 數據操作介面
###### tags: `大數據` `HTML`

## what is HTML

### 最初設計是傳送文件

### HTML 架構

![](https://i.imgur.com/BtIHeXq.png)

* head : 經常放一些設定資料
* body : 放內容

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

## 軟體介紹
* 軟體名稱 : VisualStudio Code

## 開始寫網頁
1. 新建資料夾
    ![](https://i.imgur.com/ijPxWgL.png)
2. 開啟VisualStudio Code
    ![](https://i.imgur.com/jQgadQq.png)
1. 開啟剛剛的資料夾
    ![](https://i.imgur.com/FdSydPh.png)
1. 建立html，在左側點右鍵，選新增檔案
    ![](https://i.imgur.com/ucMRV8k.png)
1. 輸入first.html
    ![](https://i.imgur.com/WavcJub.png)
1. 在右邊輸入html，會出現提示，或是直接輸入!後再按tab，就會直接出現
    ![](https://i.imgur.com/eES0lpD.png)
1. 完成後的畫面
    ![](https://i.imgur.com/jLnwryj.png)
1. 在<BODY>跟</BODY>貼上內容
    ![](https://i.imgur.com/EgypWwA.png)
1. 到資料夾內點兩下剛剛的first.html直接打開，就可以看到網頁了
    ![](https://i.imgur.com/XCmDCYA.png)


## 常用HTML語法介紹

### `<h1>到<h6>`

* 解釋 :
    代表各種不同大小的標題。
* 程式碼 : 
    ```
    <h1>This is heading 1</h1>
    <h2>This is heading 2</h2>
    <h3>This is heading 3</h3>
    <h4>This is heading 4</h4>
    <h5>This is heading 5</h5>
    <h6>This is heading 6</h6>
    ```
* 網頁呈現效果 : 
    <h1>This is heading 1</h1>
    <h2>This is heading 2</h2>
    <h3>This is heading 3</h3>
    <h4>This is heading 4</h4>
    <h5>This is heading 5</h5>
    <h6>This is heading 6</h6>

### `<p>`

* 解釋 :
    一段文字。
* 程式碼 : 
    ```
    <p>This is a paragraph.</p>
    <p>This is another paragraph.</p>
    ```
* 網頁呈現效果 : 
    <p>This is a paragraph.</p>
    <p>This is another paragraph.</p>

### `<a>`

* 解釋 :
    一段連結。
* 程式碼 : 
    ```
    <a href="https://www.w3schools.com">This is a link</a>
    ```
* 網頁呈現效果 : 
    <a href="https://www.w3schools.com">This is a link</a>
    

### `<img>`

* 解釋 :
    用於在 HTML 頁面中嵌入圖像。
* 程式碼 : 
    ```
    <img src="https://miro.medium.com/max/1352/1*XEgA1TTwXa5AvAdw40GFow.png">
    ```
* 網頁呈現效果 : 
    <img src="https://miro.medium.com/max/1352/1*XEgA1TTwXa5AvAdw40GFow.png">
    
### `<table>`

* 解釋 :
    產生表格。
* 程式碼 : 
    ```
    <table>
      <tr>
        <th>Month</th>
        <th>Savings</th>
      </tr>
      <tr>
        <td>January</td>
        <td>$100</td>
      </tr>
      <tr>
        <td>February</td>
        <td>$80</td>
      </tr>
	</table>
    ```
* 網頁呈現效果 : 
    <table>
      <tr>
        <th>Month</th>
        <th>Savings</th>
      </tr>
      <tr>
        <td>January</td>
        <td>$100</td>
      </tr>
      <tr>
        <td>February</td>
        <td>$80</td>
      </tr>
	</table>
    
### `<ol>`

* 解釋 :
    自動排序列表。
* 程式碼 : 
    ```
    <ol>
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
    </ol>

    <ol start="50"> 從50開始計數
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
    </ol>
    ```
* 網頁呈現效果 : 
    <ol>
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
    </ol>

    <ol start="50">
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
    </ol>
    
### 還有許多tag可以查閱W3CSchool

https://www.w3schools.com/tags/tag_a.asp

![](https://i.imgur.com/As3FkwS.png)

## Styles
許多html tag裡都可以加上Style來改變顯示外觀。
### `<background-color>`

* 解釋 :
    背景顏色。
* 程式碼 : 
    ```
    <h1  style="background-color:powderblue;">This is a heading</h1>
    <p  style="background-color:red;">This is a paragraph.</p>

    ```
* 網頁呈現效果 : 
    <h1  style="background-color:powderblue;">This is a heading</h1>
    <p  style="background-color:red;">This is a paragraph.</p>

### `<Text Color>`

* 解釋 :
    字體顏色。
    
* 程式碼 : 
    ```
    <h1 style="color:blue;">This is a heading</h1>
    <p style="color:red;">This is a paragraph.</p>
    ```
    
* 網頁呈現效果 : 
    <h1 style="color:blue;">This is a heading</h1>
    <p style="color:red;">This is a paragraph.</p>

### `<font-family>`

* 解釋 :
    字型。
    
* 程式碼 : 
    ```
    <h1 style="font-family:verdana;">This is a heading</h1>
    <p style="font-family:courier;">This is a paragraph.</p>
    ```
    
* 網頁呈現效果 : 
    <h1 style="font-family:verdana;">This is a heading</h1>
    <p style="font-family:courier;">This is a paragraph.</p>

### `<Text Size>`

* 解釋 :
    字體大小。
    
* 程式碼 : 
    ```
    <h1 style="font-size:300%;">This is a heading</h1>
    <p style="font-size:160%;">This is a paragraph.</p>
    ```
    
* 網頁呈現效果 : 
    <h1 style="font-size:300%;">This is a heading</h1>
    <p style="font-size:160%;">This is a paragraph.</p>
    
## CSS
* CSS 可以值寫皆訂一整頁的樣式，節省了大量工作，不必在每個html tag裡加上style。它可以同時控制多個網頁的佈局 外部樣式表存儲在 CSS 文件中

### 透過tag控制

* 程式碼 : 
    ```
    <!DOCTYPE html>
    <html>
    <head>
    <style>
        body {
          background-color: lightblue;
        }

        h1 {
          color: white;
          text-align: center;
        }

        p {
          font-family: verdana;
          font-size: 20px;
        }
    </style>
    </head>
    <body>

    <h1>My First CSS Example</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>
    ```
    
* 網頁呈現效果 : 
![](https://i.imgur.com/xe5BWx4.png)

### 透過自訂class控制

* 程式碼 : 
    ```
    <!DOCTYPE html>
    <html>
    <head>
        <style>
            .intro {
              background-color: yellow;
            }
        </style>
    </head>
    <body>

        <h1>Welcome to My Homepage</h1>

        <div class="intro">
          <p>My name is Donald.</p>
          <p>I live in Duckburg.</p>
        </div>

        <p>My best friend is Mickey.</p>

        <p class="intro">My best friend is Mickey.</p>

    </body>
    </html>
    ```

* 網頁呈現效果 : 
    ![](https://i.imgur.com/vYTIN0N.png)

### 透過tag + 自訂class控制

* 程式碼 : 
    ```
    <!DOCTYPE html>
    <html>
    <head>
        <style>
            p.center {
              text-align: center;
              color: red;
            }

            p.large {
              font-size: 300%;
            }
        </style>
    </head>
    <body>

        <h1 class="center">This heading will not be affected</h1>
        <p class="center">This paragraph will be red and center-aligned.</p>
        <p class="center large">This paragraph will be red, center-aligned, and in a large font-size.</p> 

    </body>
    </html>

    ```

* 網頁呈現效果 : 
    ![](https://i.imgur.com/ReglksY.png)

## 回家作業
* 網頁呈現效果 : 
    
    ![](https://i.imgur.com/J2GpMZv.jpg)

* 程式碼 : 
    ```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <style>
            body{
                font-family: "標楷體";
            }
            .container{
                width: 1200px;
                margin-left: auto;
                margin-right: auto;
            }
            .box{
                width: 100px;
                margin-left: auto;
                margin-right: auto;
            }
            h1{
                color: blueviolet;
                text-align: center;
            }
            h2{
                color:rgb(240, 89, 8);
            }
            td, th{
                width: 150px;
                text-align: center;
            }
            table{
                background-color: cyan;
            }
            .green{
                background-color: rgb(192, 250, 104);
            }
            ol.b {list-style-type: cjk-ideographic;}
        </style>
    </head>
    <body>
        <div class="container">

    <h1>當你心情不好的時候..看看</h1>
    <h2>不說話</h2>
    <p>
    有時候，你被人誤解，你不想爭辯，所以選擇沈默。本來就不是所有的人都得了解你，因此你認為不必對全世界喊話。卻也有時候，你被最愛的人誤解，你難過到不想爭辯，也只有選擇沈默。全世界都可以不懂你，但他應該懂，若他竟然不能懂，還有什麼話可說?生命中往往有連舒伯特都無言以對的時刻，畢竟不是所有的是非都能條列清楚，甚至可能根本沒有真正的是與非。那麼，不想說話，就不說吧，在多說無益的時候，也許沈默就是最好的解釋。
    </p>
    <h2>至少要平靜</h2>
    <p>
    在你跌入人生谷底的時候，你身旁所有的人都告訴你：要堅強，而且要快樂。堅強是絕對需要的，但是快樂?在這種情形下，恐怕是太為難你了。畢竟，誰能在跌得頭破血流的時候還覺得高興？但是至少可以做到平靜。平靜地看待這件事，平靜地把其他該處理的事處理好。平靜，沒有快樂，也沒有不快樂。能做到這一點，你就已經有了復元的能量。
    </p>
    <h2>彎腰</h2>
    <p>
    和別人發生意見上的紛歧，甚造成言語上的衝突，所以你悶悶不樂，因為你覺得都是別人惡意。別再耿耿於懷了，回家去擦地板吧。拎一塊抹布，彎下腰，雙膝著地，把你面前這張地板的每個角落來回擦拭乾淨。然? 嵾奐s省思自己在那場衝突，所說過的每一句話。現在，你發現自己其實也有不對的地方了，是不是?你漸漸心平氣和了，是不是?有時候你必須學習彎腰，因為這個動作可以讓你謙卑。勞動身體的同時，你也擦亮了自己的心緒。而且，你還擁有了一張光潔的地板呢。這是你的第二個收穫。
    </p>
    <h2>如果當初</h2>
    <p>
    你說，人生是一條有無限多岔口的長路，永遠在不停地做選擇。如果只是選擇吃炒麵或炒飯，影響似乎不大，但選擇讀什麼科系、做什麼工作、結婚或不結婚、要不要有孩子，每一個選擇都影響深遠，而不同的選擇也必定造就完全不一樣的人生。你又說，生命中不可承受之情，就在於人生沒有重來的機會啊。如果當初如何如何，現在就不會怎樣怎樣........，這種充滿悵然的喃喃自語，還是別再多說了吧。每一個岔口的選擇其實沒有真正的好與壞，只要把人生看成是自己。獨一無二的創作，就不會頻頻回首如果當初做了不一樣的選擇。
    </p>
    <h2>曾經美麗</h2>
    <p>
    漫步林間，你看見一株藤蔓附著樹幹，柔軟與堅實相互交纏，你感?囥馧o靜美的一幕。讓幸福與歸屬就此駐足吧。你想。不知未來會有怎樣一番風雨摧折？也許藤將斷、樹會倒，也許天會荒，地將老。你又想。那麼，請時光停格在此刻吧。
    停 ? 瑽Y是永恆。永恆裡若有這靜美的一刻，未來可能遭遇的種種劫難，便已得到了安慰與報償。
    </p>
    <h2>覆滿藤蔓的屋頂</h2>
    <p>
    你希望擁有一片斜斜的屋頂，屋頂上爬滿了青綠的藤蔓，藤蔓裡結出纍纍絲瓜。夏日傍晚，天起涼風的時刻，你爬上靠牆的木梯，到屋頂上採收一顆被陽光烘熟的瓜。然後，你來到廚房， 煮一鍋美清淡的蛤蜊絲瓜湯。「多好啊，」你無限嚮往:「如果我擁有一片覆滿藤蔓的屋頂......」事實上，你已經擁有了----在想像裡。無論現實多樣燥熱擾攘，只要能夠想像，你就可以維持內在 的平靜清涼，這種自在的滋味，嗯，也許正如你一個人靜靜地喝一碗蛤蜊絲瓜湯。
    </p>
    <h2>單純</h2>
    <p>
    因為思慮過多，所以你常常把你的人生複雜化了。明明是活在現在，你卻總是念念不忘著過去，又憂心忡忡著未來 ；堅持攜帶著過去、未來與現在同行，你的人生當然只有一片拖泥帶水。而單純是一種恩寵狀態。單純地以皮膚感受天氣的變化，單純地 以鼻腔品嘗雨後的青草香，單純地以眼睛統攝遠山近景如一幅畫。單純地活在當下。而當下其實無所謂是非真假。既然沒有是非，就不必思慮；沒有 真?瓷A就無須念念不忘又憂心忡忡。無是非真假，不就像在做夢一樣了嗎?是呀，就單純地把你的人生當成夢境去執行吧。
    </p>
    <h2>偶爾</h2>
    <p>
    吃多了健康食品，偶爾你也想啃一啃鴨舌頭和鹽酥雞。看多了大師名劇，偶爾你也想瞄一瞄耳光摔不完眼淚掉不完的連續劇。聽多了古典音樂，偶爾你也想唱一唱愛他一百年又恨他一他一萬年的流行歌曲。你知道健康食品對健胃整腸有意義，大師名劇對培養氣質有意義，古典音樂對提升性靈有意義，可是，偶爾你其實並不想讓自己時時刻刻活得那麼有意。人生不需要把自己綁得那麼緊。偶爾的小小放縱，是道德的。靈氣充滿或許接近大人，但偶爾的俗氣會更平易近人。
    </p>
    <h2>別浪費了</h2>
    <p>
    今天的你，是不開心的你，因為有人在言語間刺傷了你。你不喜歡吵架，所以你離開；可是你只是離開了那，卻沒有離開被那人傷害的情境，因此你愈想愈生氣。愈有氣，你就愈沒有力氣去理會別的事情，許多更該用心去做去想去處理的事件，就在你漫天漫地的心煩意亂之中，被輕忽被漠視被省略了。因為，你只是一心一意地在生氣。在情緒上做文章，這是對自己的浪費，而且是很壞的浪費。畢竟，生氣也是要花力氣的，而且生氣一定傷元氣。所以，聰明的你，別讓情緒控制
    </p>
    <h1>我個人資訊</h1>
    <h2>上課三不準則</h2>
    <div class="box">
        <ol  class="b green">
            <li>不遲到</li>
            <li>不早退</li>
            <li>不當人</li>
        </ol>
    </div>
    <h2>我的交友原則</h2>
    <ul  class="green">
        <li>有讀</li>
        <li>有回</li>
        <li>有按讚</li>
    </ul>
    <h2>我的課表</h2>
    <table border='1px' cellspacing='0'>
        <tr><th></th><th>星期ㄧ</th><th>星期二</th><th>星期三</th><th>星期四</th><th>星期五</th></tr>
        <tr><th>第一節</th><td>國語</td><td>數學 </td><td>英語</td><td>家政</td><td>電腦</td></tr>
        <tr><th>第二節</th><td>國語</td><td>數學 </td><td>英語</td><td>家政</td><td>電腦</td></tr>
        <tr><th>中場休息</th><td></td><td> </td><td></td><td></td><td></td></tr>
        <tr><th>第三節</th><td>國語</td><td>數學 </td><td>英語</td><td>家政</td><td>電腦</td></tr>
    </table><br><br>

    <table class="green" border='1px' cellspacing='0'>
        <tr><th colspan=6>我的課表</th></tr>
        <tr><th></th><th>星期ㄧ</th><th>星期二</th><th>星期三</th><th>星期四</th><th>星期五</th></tr>
        <tr><th>第一節</th><td rowspan=3>國語</td><td rowspan=3>數學 </td><td rowspan=3>英語</td><td rowspan=3>家政</td><td rowspan=3>電腦</td></tr>
        <tr><th>第二節</th></tr>
        <tr><th>第三節</th></tr>
    </table><br><br>
    <h2>我工作的地方</h2>
    <a href="https://www.mdu.edu.tw">明道大學</a><br><br>
    <img src="img/mdu.jpg" alt="明道大學" width="300px">

    </div>
    </body>
    </html>
    ```