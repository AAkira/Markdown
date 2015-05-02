# How to write the markdown

##見出し

* h1  
	\# 見出し
* h2  
	\## 見出し
* h3  
	\### 見出し
* h4  
	\#### 見出し

* max:6
* 行末でもok

## 段落と改行

* 段落
 - 空白行で囲まれた1行
 - 複数行の文章
 - 改行が入っていても1行以上の空白が入っていなければ1つの段落

* 複数行で改行を入れたい場合
 - 半角スペースを2つ以上入れる

## 強調

* アスタリスクを1つ並べる(em)  
 \*strong word\*  
 例) hoge*Strong*hoge

* アンダーバーを1つ並べる(em)  
 \_strong word\_

* アスタリスクを2つ並べる(strong)  
 \*\*strong word\*\*  
 例) hoge**Strong**hoge

* アンダーバーを2つ並べる(strong)  
 \_\_strong word\_\_

## 打ち消し

* 波線2つで囲う  
 \~~hoge~~  
 例) You ~~am~~ are hoge.

## リスト

* \*, \-, \+の後ろにスペースorタブを挿入  

 \* list1  
 \* list2  
 \+ list3  
 \- list4  
* リストの途中でスペースorタブを入れて記号を変更すると入れ子になる  

 \* list1  
 　\- innner1  
 　\- innner2  
 \+ list2  
 　\+ innner1  
 　\+ innner2  
 　\+ innner3  
 \+ list3  
 \+ list4  

* 数字+ピリオドでも可能だが数字の並べ替えは無し

 1\. list1  
 2\. list2  
 9\. list3  
 6\. list4  
 3\. list5  
 4\. list6  

## 罫線

* 3つ以上の*,　-,　_,　[半角スペース]のみの行

 \*\*\*    
 \*　\*　\*　\*  
 \-------  
 \_\_\_\_  

## リンク

* <\>で囲うとそのままリンク  
	
  < http://www.google.com \>

* 角括弧[]:表示文字,丸括弧():URL  

  \[Google](http://www.google.com)  
  e.g.) [Google](http://www.google.com)

* まとめて参照  

	\[人民][a]の[人民][a]による[人民][a]のための[政治][b]  
	\[a]: http://ja.wikipedia.org/wiki/%E4%BA%BA%E6%B0%91  
	\[b]: http://www.kantei.go.jp/ "首相官邸"

* タイトルナシの画像  

 !\[alt](url)

* タイトルアリの画像  

 !\[alt](url "title")

## 引用

* \> を行頭につける
 > この文章はhogeから  
 > 引用しています。

## Code

* 逆クォーテーションで括る< code>タグと同じ  
 \`public static final String HOGE = "hogehoge"\`  

 e.g.)  
 `public static final String HOGE = "hogehoge"`

* JSON形式  
\```json [hoge] \```

 e.g.)  

```json
[
	{
		id:1234  
	}
]
```


## エスケープ

* 記号は対象文字列前に\  

* 範囲は< div> ... </ div>で囲う

## テーブル

* テーブルの線によって寄せが変わる  

 \|指定なし|左寄せ|中央寄せ|右寄せ|  
 \|--------|:-----|:------:|-----:|  

 \|  hogehoge  |   foofoo    |    barbar    |  
 \|:-----------|------------:|:------------:|  
 \| hogehoge   | foo         |bar           |  
 \| hoge       |      foo    |    bar       |  
 \| hoge       |  foo        |          bar |  
 \|      hoge  |          foo|           bar|  


 |  hogehoge  |   foofoo    |    barbar    |
 |:-----------|------------:|:------------:|
 | hogehoge   | foo         |bar           |
 | hoge       |      foo    |    bar       |
 | hoge       |  foo        |          bar |
 |      hoge  |          foo|           bar|

* 省略形
 
 指定無し|左寄せ|中央寄せ|右寄せ  
 -|:-|:-:|-:

