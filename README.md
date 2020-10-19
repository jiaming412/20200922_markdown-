# hankMD 功能大略

## 開會時間
- 1th 2020/09/23 14:00
  - 開會內容:
- 2th > 待約
> 引用1
>> 引用2
>>> 引用3
>>> 
*斜體*
**粗體**
![](https://hackmd.io/favicon.png)
{%youtube Hk7dQWgg-vE %}
![](https://i.imgur.com/Whlgf39.jpg)
https://hackmd.io/@jiaming412/S1LfKTlBD
```htl
<iframe width="70%" height="900" src="https://hackmd.io/features" frameborder="0"></iframe>
```
[TOC]
### Speakerdeck
{%speakerdeck sugarenia/xxlcss-how-to-scale-css-and-keep-your-sanity %}

### PDF
**注意：請使用 https 的網址，否則可能會被您的瀏覽器阻擋載入**
{%pdf https://www.w3.org/TR/WAI-WEBCONTENT/wai-pageauth.pdf %}

## UML 圖表

### 循序圖

您可以像是以下使用循序圖：

```sequence
艾莉絲->包柏: 哈摟，你好嗎？
Note right of 包柏: 包柏思考中
包柏-->艾莉絲: 我很好，謝謝！
Note left of 艾莉絲: 艾莉絲回應
艾莉絲->包柏: 最近過得怎樣？
```

### 流程圖

您可以像是以下使用流程圖：
```flow
st=>start: 開始
e=>end: 結束
op=>operation: 我的操作
op2=>operation: 啦啦啦
cond=>condition: 是或否？

st->op->op2->cond
cond(yes)->e
cond(no)->op2
```

### Graphviz
```graphviz
digraph hierarchy {

                nodesep=1.0 // increases the separation between nodes
                
                node [color=Red,fontname=Courier,shape=box] //All nodes will this shape and colour
                edge [color=Blue, style=dashed] //All the lines look like this

                Headteacher->{Deputy1 Deputy2 BusinessManager}
                Deputy1->{Teacher1 Teacher2}
                BusinessManager->ITManager
                {rank=same;ITManager Teacher1 Teacher2}  // Put them on the same level
}
```

### Mermaid
```mermaid
gantt
    title A Gantt Diagram

    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    anther task      : 24d
```
### Mermaid
```mermaid
gantt
dateFormat  YYYY-MM-DD
title Adding GANTT diagram to mermaid
excludes weekdays 2014-01-10

section A section
Completed task            :done,    des1, 2014-01-06,2014-01-08
Active task               :active,  des2, 2014-01-09, 3d
Future task               :         des3, after des2, 5d
Future task2               :         des4, after des3, 5d
```

### Vega-Lite
```vega
{
  "$schema": "https://vega.github.io/schema/vega-lite/v4.json",
  "data": {"url": "https://vega.github.io/editor/data/barley.json"},
  "mark": "bar",
  "encoding": {
    "x": {"aggregate": "sum", "field": "yield", "type": "quantitative"},
    "y": {"field": "variety", "type": "nominal"},
    "color": {"field": "site", "type": "nominal"}
  }
}
```

警告區塊
---
:::success
耶 :tada:
:::

:::info
這是訊息 :mega:
:::

:::warning
注意 :zap:
:::

:::danger
喔不 :fire:
:::

:::spoiler 點選顯示更多內容
找到我了！ :stuck_out_tongue_winking_eye:
:::

:::spoiler {state="open"} 預設展開摺疊內容
找到我了！ :stuck_out_tongue_winking_eye:
:::

#### 項目

+ 在行開頭使用 `+` `-` 或是 `*` 來建立清單
+ 空兩個空白就可以產生子清單
  - 當清單標記使用的字元不同，會強制建立新的清單
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ 非常簡單！

#### 編號

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
1. 您可以逐次增加項目數字...
6. 5454
7. 848

 程式碼:


    // sodkoksd
    484848
    15121
    
    
### 連結
[連結文字](http://dev.nodeca.com)
[加上標題的連結文字](http://nodeca.github.io/pica/demo/ "標題文字！")
自動轉換連結 https://github.com/nodeca/pica

![Minion](https://octodex.github.com/images/minion.png "哈哈幹你娘" =200x200 )
使用指定的大小顯示圖片
    
    
---------
    
# 以下是練習唷~~

## PERT圖

```graphviz
digraph {
node[shape=record];
rankdir="LR";
struct1 [label="設計UI |{{ 開始日:|結束日:}| { 編號:1|需時:}}"];
struct2 [label="取得授權|{{ 開始日:|結束日:}| { 編號:2|需時:}}"];
struct3 [label="電路板設計|{{ 開始日:|結束日:}| { 編號:3|需時:}}"];
struct4 [label="安裝&測試|{{ 開始日:|結束日:}| { 編號:4|需時:}}"];
struct5 [label="提案|{{ 開始日:|結束日:}| { 編號:5|需時:}}"];
struct1:f1 -> struct2:f0;
struct1:f0 -> struct3:f1;
struct2:f0 -> struct4:f1;
struct3:f0 -> struct4:f1;
struct4:f0 -> struct5:f1;
}
```



   

