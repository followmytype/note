# markdown 使用筆記
## 標題字
在想要的標題文字前加個#
```md
# 這是最大標<h1>
## 幾個井字號就代表<h幾>
```
# 大標
### 換行
若在一個段落裡面想要換行  
在句尾加上兩個空白再按enter即可
___
### 行分隔符號
三個以上的星號、減號、底線 可以建立一個分隔線 但是行內不能有其他東西
```md
***
---
___
```
___
### 粗體&斜體
若要用斜體用星號或底線括起*字串*  
粗體用兩個星號或底線包起**字串**  
刪除線則用兩個波浪符圈起~~字串~~
```md
*斜體*
_斜體_
**粗體**
__粗體__
~~刪除線~~
```
___
### 列表清單
在每個列表清單項目前加上 * + 或 -   
若要有序輸出表單則用數字加英文句點  
換行的時候建議縮排會比較好看 但是不用也沒差  
數字亂打不影響結果有序的輸出
```md
* 列表一
* 列表二
  * 列表二之一
  * 列表二之二
    * 同樣邏輯新增列表
1. 第一點
2. 第二點
```
* 列表一
* 列表二
  * 列表二之一
  * 列表二之二
    * 列表二之二之一
1. 第一點
   1. 一之一
   2. 一之二
2. 第二點
___
### checkBox
- [x] 吃飯
- [x] 工作
- [ ] 睡覺
```md
- [x] 這是代表已選取
- [ ] 這是沒有被選取的
```
___
### 程式碼區塊
圈出一個程式碼區塊有兩種方式  
* 前面有四個空白
* 或是用三個反引號圈出區塊(前面可以指定程式語言)
* 若要在行內標記程式碼，則用單個反引號圈起來  
  譬如我都用`console.log(error)`來做js的除錯
```
    大區塊前面加四個空白
```
    ```php
    $str = 'Hello World';
    echo $str;
    ``` 
```
`使用一個反引號圈起行內程式碼`
```
___
### 連結&圖片
#### 連結  
* 用方括號標記，後面用小括號插入網址，若要加上連結`title`只需要在網址後面雙引號括起來就好了，[我的GitHub](https://github.com/followmytype "漸漸在經營了")。
#### 圖片  
* 產生圖片的方式跟連結一樣，但前面要加個驚嘆號
  ![Google圖片](https://ssl.gstatic.com/images/branding/googleg/2x/googleg_standard_color_64dp.png)可惜不能指定圖片大小
```md
[連結文字](網址 "連結標題")
等同
<a href='網址' title='連結標題'>連結文字</a>

![圖片文字](網址)
```
#### 文末連結引用
* 若是一段落句內包含許多其他連結，譬如[Google], [Yahoo], [Msn]這   些常用連結，若是用上面的方法會顯得混亂，可以用引用的方式，在文章的    最末端補上連結，大小寫沒關係
```md
[Google], [Yahoo], [Msn]
> 文章最後補上
[google]: http://google.com/        "Google"
[yahoo]: http://search.yahoo.com/  "Yahoo Search"
[msn]: http://search.msn.com/    "MSN Search"
```
#### 自動連結
* 用<>括起網址就能自動連結了，譬如<https://www.google.com/>
```md
<https://www.google.com/>
```
___
### 階層區塊
若要使用引言的話 可以使用階層區塊的方式  
用 > 代表階層，幾個 > 代表第幾層
> 第一層
>> 第二層  
>> 這裡還是在第二階
>>> 這樣就進入到第三階了
>> 
>> 第二層
```md
> 第一層
>> 第二層  
>> 第二層
>>> 第三層
>>
>> 第二層
```
___
### 表格
用減號以及豎號做出表格

|name|age|gender|
|----|---|------|
|Matt|22 |male  |
|Mina|19 |female|
* :--- 靠左對齊  
* :--: 置中對齊  
* ---: 靠右對齊

|left|center|right|
|:---|:----:|----:|
|aa  |bb    |cc   |
|靠左 |置中  |靠右  |
```md
|name|age|gender|
|----|---|------|
|Matt|22 |male  |
|Mina|19 |female|
******************
|left|center|right|
|:---|:----:|----:|
|aa  |bb    |cc   |
|靠左 |置中   |靠右 |
```
___
詳細寫法請看mkdown_note.txt  

[google]: http://google.com/        "Google"
[yahoo]: http://search.yahoo.com/  "Yahoo Search"
[msn]: http://search.msn.com/    "MSN Search"