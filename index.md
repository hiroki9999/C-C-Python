# GitHubとは
まず、こうして閲覧しているこのサイトであるGitHubとは何なのか公式ガイドに以下のうように定義されています。  
GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.  
簡単にいうとGitHubとは自身がプログラミングを他のプログラマーにも共有することができるサービスのことを指します。  
  
GitHubとは何かを理解したところで早速プログラミング言語について学んでいきます。
プログラミング言語は大きく分けて二つの言語が存在します。  
一つはインタプリンタ言語、もう一つはコンパイラ言語です。  
  
この二つの言語には大きな違いが存在しその違いから速度や容易さが変化します。  
インタプリンタ言語では打ち込んだプログラミング言語を一つ一つ機械語に変換しコンピュータがソースコードを実行をします。
コンパイラ言語では機械語をそのままプログラミング言語として打ち込みコンピュータがソースコードを実行します。 
  
すごく簡単に言うと、インタプリンタ言語は理解しやすく動作が遅い。コンパイラ言語では理解が難しいが動作が速いという特徴があります。
また、それに加えてインタプリンタ言語ではコンピュータが一つ一つ解釈するためどの部分に問題があるのかをコンパイラ言語よりも簡単に把握できるメリットも存在します。
インタプリンタ言語の代表例はPython, HTML  
コンパイラ言語の代表例はC, C++,   

今回、中心的に学んでいくPythonはインタプリンタ言語に属しています。

# Pythonについて
前の章でも説明したようにPythonはインタプリンタ言語であるためはじめにインタプリンタ（通訳者）を起動する必要があります。  


# Pythonの使い方
プログラミングを始めるうえで最も大切なことは
"より簡潔にわかりやすくプログラムを書くこと"です。
誰が見ても理解できるようなプログラムを書くことがプログラマーには求められます。  
そのためにプログラム内でコメントを表示する必要があります。
Pythonでは"#"ハッシュタグを文頭に置くことでその文をコメントとしてプログラム内のみで表示することができます。もちろん＃内の内容はプログラムには影響を及ぼしません。
# Pythonでの計算
では、実際にPythonを動かすプログラムを書いていきます。まず、Pythonを電卓として利用する方法を解説します。
インタプリンタ内では式をそのまま入力することで結果が次の文に表示されます。  
プログラム内では演算子を次のように表します。  

|Type|Purpose|Example|Result|
|---|---|---|---|
|+|和(足す)|1 + 1|2|
|-|差(引く)|2 - 1|1|
|*|積(かける)|2 * 9|18|
|/|商(割る)|9 / 2|4.5|
|%|余剰を示す|9 % 2|1|
|//| 整数徐算(少数切り捨て)|9/2|4|


また、プログラム内でも計算順序は同様に右から左を基本に"()"カッコ内、掛け算と割り算、足し算と引き算の順に計算をしていきます。  
一つ注意が必要な点は整数を扱う（int）型と小数点を持つ（float）型が存在することです。
この他にもdecimal型: 浮動小数点を自ら定義、fraction型: 分数の保持、complex型: 複素数が存在します。    
int型とfloat型の計算ではfloat型が優先されるため2*2*3.5=14.0という結果が返されます。 
次に、少し発展的な演算子について紹介します。

|Type|Purpose|Example|Result|
|---|---|---|---|
|abs()|絶対値|abs(-1)|1|
|int()|整数への変換|int(3.14)|3|
|float()|浮動小数点数への変換|float(3)|3.00|
|complex(,)|複素数化|complex(5,3)|5+3j|
|divmod(,)|整数の商と余り|divmod(9,2)|(4,1)|
|pow(,)|累乗|pow(2,5)|32|
|**|累乗|2**5|32|
|math.trunk()|小数点切り捨て|math.trunk(-19.5)|-19|
|math.floor()|小数点切り捨て|math.floor(-19.5)|-20|
|math.ceil()|小数点切り上げ|math.ceil(11.1)|12|
|round()|四捨五入|round(1.5)|2|

次に変数の代入について説明します。  
プログラミング内では同じ数字や表現を何度も使うことがほとんどです。  
そのために"="を利用します。  

|Type|Purpose|Example|Result|
|---|---|---|---|
|isdigit()|数字かどうかを評価する。float型はFalse|print"0".isdigit()|True|
|

# Pythonで文字を打つ
Pythonは計算機だけでなく文字を打つことも可能です。  
文字列を記述する方法は''単引用符、""二重引用符で文字を囲む二種類が存在します。  
また、''' ''',""" """三連引用符を利用することで複数行にまたがって文字を打つこともできます。  
文字列は"+"演算子で連結、"＊"演算子で反復させることができます。  
連続して並んだ文字列は自動的に連結されます。
変数と文字列を使用したいときは"+"演算子を利用します。
変数で指定した文字列は左から0,1,2,3...右から-1,-2,-3,...の順で数えられ変数の後に[]を加えることで番号にあった文字列を表示することができます。
また、変数内で表示する文字列を
以下割愛の予定。
https://docs.python.org/ja/3/tutorial/introduction.html#id4 22/09/19
Pythonの機能

|Type|Purpose|Example|
|---|---|---|
|slice|指定した番号の文字を表示する||
|len()| ()内で示した変数の文字列の長さを表示する|len(x)|
|list型|[]で囲んだ値（数字、文字）を指定した変数に保存する|list|
|if文|条件を示し条件にあった場合if文内のコードを実行させる|if x<5:|
|elif文|if文と並列して使われ、if文の条件外かつelif文の条件にあった場合コードを実行させる|elif x<10:|
|else|if、elif文などと並列して使われ、ifの条件外の時にコードを実行させる|else:|
|for文|反復を実行させる|for i in list:|
|range(x,y,z)関数|()内の数列を生成する。初めの数字をx、終わりの数字をy、z毎の数字を示す|range(1,10,2)|
|break|ifやwhileなどの繰り返しを終わらせる|break|
|continue|ifやwhileなどの繰り返しをスキップできる|continue|
|pass|何もしない。文法上必要な時に使う|pass|

# 関数の定義
def
1.デフォルト引数値  
2.キーワード引数値  
3.任意引数値リスト  
ラムダ式  
# 様々なlist型

|type|purpose|example|
|---|---|---|
|list.append(x)|リスト末に新たな要素xを追加する(変数不可)|list.append(5)|
|list.extend(x)|リスト末に新たな要素xを追加する(変数可)|list.extend(x)|
|list.insert(i,x)|指定した位置iに新たな要素xを追加する|list.insert(0,0)|
|list.remove(x)|リスト内にある要素xを削除する|list.remove(5)|
|list.pop([i])|リスト内の指定された位置iにある要素を削除し表示する|list.pop([0])
|a.pop()|リスト末の要素を削除して表示する|a.pop()|
|list.clear()|リスト内の全ての要素を削除する|list.clear()|(del a[]と同等)
|list.index(x[s[e]])|リスト内でxと等しい値を持つ要素の位置を表示する[s[e]]ではsからeまでの範囲内でxの位置を示す|list.index(2)|
|list.count(x)|リスト内でのxの出現回数を表示する|list.count(1)|
|list.sort(key=Npme, reverse=False)|リストの項目を||
|list.reverse()|リストの順序を逆にする|list.reverse()|
|list.copy()|リストのコピーを示す|list.copy|(a[:]と同等)

del文: listなどの内容を削除することができる。  
# Sequenceデータ型
Sequenceデータ型: list, tuple, rangeの  

|Type|Purpose|Example|Result|  
|---|---|---|---| 
|x in s|sの中にxが含まれているとTrue、なければFalse|a in banana|True|  
|x not in s|sの中にxが含まれていないとTrue、いるとFalse|a not in banana|False|  
|s + t|
|s * n|
|s[i]|
|s[i:j]|
|s[i:j:k]|
|len(s)|
|min(s)|
|max(s)| 
|s.index(x[,i[,j]])|
|s.count(x)|

# タプルtaple型とリストlist型
タプル-taple型  
```Python
t = 12345,67890,"hello"
t[0]
```
  
`12345`  
リスト-list型  
```Python
l = [12345,67890,"hello"]
l[0]
```
  
`12345`  
違い：タプル型は不変、リスト型は可変である  

# モジュール
長いプログラムや複数のプログラムを動かすためにはスクリプトの作成が必須でありそのためにはモジュールという概念を知る必要があります。  
モジュールとはプログラムの定義を収めるところです。  
モジュールの概念を理解するためにはオブジェクト指向という考え方を知る必要があります。  
ところで、今回のこのPythonの説明文はとても簡単なオブジェクト指向によって書かれています。
この文章だけでなく普段読む本やネットに記載されている記事などもオブジェクト指向によって書かれていると思っています。  
では、オブジェクト指向とは何なのか。私は目次がオブジェクト指向であると考えています。  
目次を見るだけでその本のどのページに何が書かれていてその本の内容のあらすじが書いてあります。  
そのため目次（モジュール）を読むことでその本や記事（プログラム）の内容を理解することができるのです。    
そして、その目次（モジュール）に書いてあるページに飛ぶことで本の内容（スクリプト）にたどり着くことができるのが簡単なオブジェクト指向の考え方です。  
  
次にモジュール内の定義を呼び出す方法を解説します。  
モジュールとは先に説明したようにスクリプトを呼び出すための目次のようなものです。  
目次を呼び出すためには目次内の内容がなくてはなりません。  
import: モジュール内でスクリプトを見つけ出し、プログラム内で定義する。  
from import: fromでモジュールを見つけ出しimportで内容を複数選択が可能。  
importの後に*をつけるとモジュール内のもの全てがインポートされる。（未知の名前が定義されてしまうため注意が必要。）  
  
ここに関してはクラスでより深く言及していく予定です。  
  
import as: importした内容をasの後に書く名前でも定義できるようにしたもののことを指します。
from import as も同様です。  
　　
dir()関数: モジュール内の名前の定義を調べる    
パッケージ: モジュールの名前を構造化する手段。複数のプログラマが協力するときに有効  
新しい概念であるパッケージが出現しました。  
パッケージとは簡単に説明するとモジュールの集合体です。  
パッケージがモジュールの集合体でモジュールがクラスの集合体でクラスがメソッドの集合体、、、  
よくわからないので図にしてみると  
パッケージ＞モジュール＞クラス＞メソッド  
ということになります。
　　
使用例：import sound.effects.echo
　　
# 入力と出力

式文  
print()  
write()  
文頭にf,F文中に{}  
str.format()  
str(): 人間に読める表現を返す  
repr(): インタプリンタに読める表現を返す  

フォーマット済みリテラル
: をつけると最小の文字幅を指定できる

format()メソッド
print内にある{}の中身を打ち込むことができる  
   
```Python  
>>> for x in range(1, 11):'
...     print('{0:2d} {1:3d} {2:4d}'.format(x, x*x, x*x*x))
...
 1   1    1
 2   4    8
 3   9   27
 4  16   64
 5  25  125
 6  36  216
 7  49  343
 8  64  512
 9  81  729
10 100 1000
```

文字列の手作業でのフォーマット

str.rjust(): 指定された幅のフィールド内に文字列が右寄せで入るように左側に空白を追加する  
str.ljust(): 左寄せで入るよう右側に空白を追加  
str.center(): 中央寄せ  
str.zfill(): 左側をゼロ詰め  
　　
ファイルの読み書き
open(,): ファイルオブジェクトを開く。open(ファイル名,Mode)with文を使うのがおすすめ  
  
|Mode|Purpose|Example|
|---|---|---|
|r|読み取り（デフォルト）|open("sample.txt","r")|
|w|書き込み|open("sample.txt","w")|
|a|生成？|open("sample.txt","a")|
|b|バイナリモード|open("sample.txt","b")|
|t|テキストモード（デフォルト）|open("sample.txt","t")|
|+|読み取り＋書き取り|open("sample.txt","w+")|
  
sample.txt
```Python
First line
Second line
Third line
Forth line
```
  
[read()メソッド](https://yukun.info/python-file): ファイルを読み込み、文字列データに対して処理を行う  
  
```Python
f = open("sample.txt" , "r")
data1 = f.readline(1)
data2 = f.readline(2)
data = f.readline()

print(data1)
print(data2)
print(data)
```
↓
F
ir
Fist line  
  
readline()メソッド: 一行ごとにファイルを読み込み処理を行う
```Python
f = open("sample.txt","r")
data1 = f.readline(1)
data2 = f.readline(2)
data = f.readline()
data3 = f.readline()
data4 = f.readline()
f.close()

print(data1)
print(data2)
print(data)
print(data3)
print(data4)
```

readlines()メソッド: ファイルを読み込み一行ごとに処理を行う
```Python
f = open("sample.txt","r")
data1 = f.readlines(1)
data2 = f.readlines(2)
data = f.readlines()

f.close()

print(data1)
print(data2)
print(data)
```
→
['First line\n']
['Secand line\n']
['Third line\n']
writelines()メソッド: ファイルの内容を書くことができる  
  
tell()メソッド: ファイルの場所を示す
37    
```Python
f = open("sample.txt","r")
f.tell()

```
seek()メソッド: 好きな場所からファイルを開始することができる
```Python


```

[with文](https://note.nkmk.me/python-file-io-open-with/): ファイルのオープンとクローズの処理を簡略化してくれる  
```Python
f = open("sample.txt", "r")
print(f.read())
f.close()
↓
with open("sample.txt", "r") as f:
    print(f.read())
```
with文を使うためには対応したクラスを作る必要があります。  
対応したクラスは_enter_()メソッドと_exit_()メソッドを定義することで作ることができます。  
  
  
# エラーと例外
エラーには構文エラーsyntax errorと例外exceptionの二種類が存在します。  
syntax errorでは基本的なプログラム構文の間違いを示します。矢印によって構文の間違いの位置を示されているためどの部分がsyntax errorなのかを判断することができます。  
exceptionではsyntax error以外の全てのエラーを示しています。たくさんの種類のexceptionが存在し、主な型は数字をゼロで割ったときに表示されるZeroDivisionErrorや定義されていない名前が使われたときのNameError、数字の型が異なったときのTypeErrorがあります。  
  
しかし、pythonではプログラム上でexceptionを起こすことが正しい場合も存在します。ではexceptionが起こった時にはどの様に処理することが正しいのでしょうか。     
  
Pythonではexceptionを処理するためにtry文を使ってプログラムを書くことができます。  
try文では例外処理を正すことが目的であるので基本的にループを利用します。
```Python
>>> while True:  
...     try:  
...         x = int(input("Please enter a number: "))  
...         break  
...     except ValueError:  
...         print("Oops!  That was no valid number.  Try again...")  
...     else:  
...         print("it's fine!")   
```
  
try文には複数のexcept（例外処理）をつけることができ、実行するプログラムの指定を行うことができexceptは例外の名称を指定してもしなくてもます。  

また、try文ではif文と同様にelseを用いることができるためexceptionが起こらないときの対応が可能です。  
  
raise文: 例外を意図的に発生させることができる。except節の中で引数のないraiseを用いることでexceptが再送出されます。つまり、定義したexceptionがもう一度発生します。
```Python
try:    
    raise ZeroDivisionError('ゼロによる除算')  
except ZeroDivisionError as eee:  
    print('eee:',eee)  
　　 raise  
```  
`eee: ゼロによる除算`
```Python
Traceback (most recent call last):  
  File "/Users/hiroki/Documents/GitHub/mypythonproject/test2.py", line 2, in <module>  
    raise ZeroDivisionError('ゼロによる除算')  
ZeroDivisionError: ゼロによる除算    
```
  
```  
try:    
    raise ZeroDivisionError('ゼロによる除算')  
except ZeroDivisionError as eee:  
    print('eee:',eee)  
```
  
`eee: ゼロによる除算`
    
→基本的に大きなプログラムなどを作ったときに例外を処理するためのクラスを作ってその中で定義するときに例外クラスを使用する。  
  
finally節: try文にはexcept,elseの他にfinally説を使用することができます。この節では名前の通り最後に処理するプログラムを支持することができます。  

# クラス

属性とはmodname.funcnameなどの"."ドットに続く名前(funcname)のことを属性と呼び、ドットよりも前の名前(modname)をオブジェクトと呼んでいます。  
属性には二つの種類（読み取り属性と書き込み）属性が存在します。    
   
ところで名前空間とはどの様なものなのでしょうか。名前空間とは簡単に言うと名前がたくさん入った箱のことです。
例えば母親に手紙を書く時に住所を書かなくては手紙は届きません。東京都という大きな箱の中の文京区のどこに住むこの人と手紙を届けるためには個人を特定するための住所が必要です。  
Pythoでも同じ様に名前空間の中に入っている名前を"定義した名前空間.名前"と入力することでのみ属性参照をすることが可能になります。  
この様に名前空間に分ける仕切りのことをスコープと呼びます。  
Pythonではスコープを三つに分けることができ、それらをbuilt-inスコープ、globalスコープ、localスコープと呼びます。  
  
built-inスコープとはPythonに元から組み込まれている組み込み関数や組み込み型を保存しているスコープのこと。  
globalスコープとはモジュール全体で使う共通の値を定義するスコープのこと。  
localスコープとはクラス内やdef内で定義するスコープのこと。  
  
nonlocal宣言: nonlocal宣言とはすぐ外側で定義されている変数をnonlocal文内で定義されている変数に設定すること
global宣言: グローバル宣言とはglovalスコープ内で変数を定義することによってその変数がglobal文内の定義をベースとして持つこと  
gloval文: localスコープ内からglovalスコープ内の変数の値を変えることができる文。  


また、Pythonでは自分で定義することができない"定数"というものが存在します。  
その定数とはNone,True,False,Notlmplemented,Ellipse,__debug__の六種類です。  
    
実はクラスを定義する方法はとても簡単なことで"class ClassName"と文を打つことでクラスを定義することができます。    
  
さて、クラスの定義ができたところで他のクラスから自分で作ったクラスを呼び出すことが可能になりました。
しかし、実際にどの様に呼び出すことができるのでしょうか。呼び出しの方法は大きく分けて三つ存在します。
今回はその三つの方法をmathクラスのpiを呼び出すものとして解説していきます。
  
(1)  
```
import math  
print(math.pi)  
```  
(2)  
```
from math import pi  
print(pi)  
  ```
(3)  
```
from math import *  
print(pi)  
  ```
ここで示した三つの例は全て同じ3.141592653589793という結果を示します。
  
次にインスタンスオブジェクトについて解説します。インスタンスオブジェクトとは変数に代入することができるもののことを指します。  
実は今まで扱ってきたクラスオブジェクトも変数に代入できるためクラスオブジェクトはインスタンスオブジェクトでもあります。  
インスタンスオブジェクトには二種類の属性名が存在します。一つ目がデータ属性、二つ目がメソッド属性です。  
一つ目のデータ属性とは  
x.counter = 1
while x.counter < 10:
    x.counter = x.counter * 2
print(x.counter)
del x.counter  
  
二つ目のメソッド属性とはappend,insert,remove,sortなどが挙げられます。  
このデータ属性とメソッド属性で名前の衝突を起こすことがしばしばあります。その時にはデータ属性が優先的にプログラム内に保存されてしまうため注意が必要です。  
  
また、メソッドオブジェクトというものも存在します。  
メソッドオブジェクトとは他の場所で保存しておいたメソッドを保存し呼び出すことができるオブジェクトのことです。  
メソッドの初めの引数ではselfという引数がよく使われています。  
  
  
では、最後にモジュールとクラスの違いについて解説します。  
クラスはモジュールに二つの機能をつけたものと考えることができます。その機能とは
1.インスタンスかしてオブジェクトを生成できること  
2.クラスから他のクラスを継承できること  
の二つです。
  
次にクラスを作ったが新しいクラスで同じ様なことを行いたい時には継承をすることでそれが可能になります。  
具体的にはクラス名を定義する時に()を置きその中に継承をしたいクラス名を書きます。すると、前のクラスで設定していたメソッドをそのまま引き継ぐことができます。  
class DerivedClassName(Base1):
また、pythonでは以下の様に記述することで多重継承をすることもできます。  
class DerivedClassName(Base1, Base2, Base3):  
新しいクラス内では継承したクラスでも使われていた変数を上書き(override)もすることができます。  
  
次に、同じオブジェクト内からのみアクセスが可能なプライベート関数について解説します。
Pythonでは  
__Name  
と名前を打つことでプライベート関数を設定することができます。
このプライベート関数は
と名前を打つことでプライベート関数を設定することができます。  
  
最後に、イテレータiteratprとジェネレータgeneratorについて学んでいきます。  
  
まず、イテレーターとは要素を一つ一つ取り出すことができるものを指します。  
また、今まで学んできたlistやdictionaryをイテレーターのコンテナオブジェクトと呼びます。  
コンテナオブジェクトを繰り返す(iterate)ことでイテレーターとして機能することができます。  
イテレーターの使用方法はnext()やfor文を使うことによって生成することができます。  
  
実際にイテレーターを使うためにはイテレータプロトコルと呼ばれるオブジェクトを実装させる必要があります。  
イテレータープロトコルとは__next()__,__iter__()のことであり、これらをdef文で定義します。  
  
```Python
...     """整数を連番で提供するイテレータクラス"""
...     def __init__(self, start, stop):
...         self._counter = start
...         self._stop = stop
...     def __iter__(self):
...         # 自分自身を返す
...         return self
...     def __next__(self):
...         if self._counter > self._stop:
...             # 最後まで到達したときは StopIteration 例外を上げる
...             raise StopIteration()
...         ret = self._counter
...         self._counter += 1
...         return ret
...     def next(self):
...         # Python 2 対応
...         return self.__next__()
```

次にイテレーターの定義は"iterator_object = iter()"と定義することでiterator_objectというイテレーターが定義されました。  
  
では、なぜイテレーターを使う必要があるのでしょうか。  
理由は二つ存在し、一つはコンテナオブジェクトの表示を簡単にするため、二つ目はメモリの節約です。  
  
では、いよいよジェネレーターについてです。  
ジェネレーターとはイテレーターを簡単に作るために作られたオブジェクトのことです。  
returnの部分をyieldに変えるだけでジェネレーターとして機能を果たすことができます。   
  
```Python
def mycounter(start, stop):
...     counter = start
...     while True:
...         if counter > stop:
...             break
...         yield counter
...         counter += 1
```    
  
# 標準ライブラリ  
標準ライブラリとは・・・？  
標準ライブラリとは何もしなくても使えるモジュール群のことを指します。  
基本的に使いたいモジュールをimportすることで使うことができます。  
授業で度々登場するmathモジュールなどが標準ライブラリの仲間です。  
  
osモジュールについて紹介していこうと思います。  
osモジュールはimport osを打ち込むことでインストールすることができます。  
肝心の機能はどの様なものがあるのでしょうか。  
osモジュールの機能はOSの機能を利用するファイルを操作するものです。  
簡単にいうと普段当たり前でやっていることをPython上で代わりに行ってくれるモジュールということです。  
例えばos.wakl()モジュールではファイルやディレクトリの一覧を取得することができ、os.system()ではunixのコマンドをpythonで記述することができます。  
また、os.path()モジュールは日頃からよく使うモジュールであるため覚えておくと便利です。 
  
|Type|Purpose|Example|
|---|---|---|
|exist()|ファイル、ディレクトリの存在確認が可能|os.path.exisr()|
|isdir()|ディレクトリの存在確認が可能|os.path.isdir()|
|isfile()|ファイルの存在確認が可能|os.path.isfile()|
|basename()|指定されたパスのファイル名を示す|os.path.basename()|  
|dirname()|指定されたパスのファイル名を除いたものを示す|os.path.dirname()|
|split()|指定されたパスのファイル名とそれまでのパスを示す|os.path.split()|
|splitext()|指定されたパスのファイル名と拡張子を示す|os.path.splitext()|
|join()|パスとファイル名などを結合することができる|os.path.join()|
  
|Type|Purpose|Example|
|---|---|---|
|walk()|ファイルやディレクトリの一覧を取得|os.walk()|
|sysrem()|UnixのコマンドをPythonで記述|os.system()|
|listdir()|ファイルやディレクトリの一覧を確認|os.listdir()|
|path()|上にて説明|os.path()|
|environ()|環境変数の取得、書き込み、上書き|os.environ()|
|mkdir()|ディレクトリの作成|os.mkdir()|
|rename()|ファイル名を変更|os.rename()|
|remove()|ファイルを削除|os.remove()|

  
また、osモジュールの他にもshutilモジュールというものも存在します。  
shutilモジュールではosモジュールではファイルの操作を行います。  
osモジュールとの違いはosモジュールではできなかったコピーや削除が可能であるということです。  
  
|Type|Purpose|Example|
|---|---|---|
|copyfile(),copy()|ファイルをコピーする（ファイルの時はcopyfile()ディレクトリの時はcopy()）|shutil.copyfile(被コピー,コピー先)|
|copyfileobj()|ファイル形式のコピー|shutil.copyfileobj()|
|copytree()|ディレクトリのまるごとコピー|shutil.copytree()|
|rmtree()|ディレクトリのまるごと削除|shutil.rmtree()|
|move()|ディレクトリの移動、リネーム|shutil.move(移動元,移動先)|
|make_archive()|zipなどのアーカイブ化|shutil.make_archive(名前,形式)|
  
  
globモジュールはファイルやディレクトリを検索することができます。
```Python
import glob
 
path_list = glob.glob('test/*.txt')
print(path_list)
```
上のコードではtestというディレクトリの中にtxtファイルがどのくらいあるかを結果で示してくれます。  
検索結果はこちら。  
`['test\\file1.txt', 'test\\file2.txt', 'test\\file3.txt']`
今回の結果ではfile1,file2,file3という三つのtxtファイルがみる借りました。
  
sysモジュールではコマンドライン引数を設定することができます。  
コマンドライン引数とはターミナルコマンドライン上からプログラムを実行するときに設定する引数のことを指します。  

まず、test.pyというファイルを作り次のコマンドを打ちます。
```Python
import sys

args = sys.argv

print(args)
print("第1引数：" + args[1])
print("第2引数：" + args[2])
print("第3引数：" + args[3])  
```  
  
コマンド上で次のプログラムを打ちます。  
python test.py a b c

すると次の結果が返ってきます。 
```Python
['test.py', 'a', 'b', 'c']
第1引数：a
第2引数：b
第3引数：c  
```  
  
このように自分で指定したファイルの中に表示させたプログラムをターミナルなどコマンドライン上で表示することができる機能をコマンドライン引数と呼びます。
同じようなものにargparseモジュールというものが存在します。  

sysモジュールには他にもsys.exit()という関数があり、これを使うことでシステムを強制的に終わらせることができます。  
  
```Python
print('おはよう')
print('こんにちは')
sys.exit()
print('こんばんは')  
```  
  
  
続いてreモジュールについて解説します。  
reモジュールは正規表現の処理を行うことができます。  
[正規表現](https://webnaut.jp/markup/606.html)とは簡単にいうと検索したい文字などの特徴を記号で表したものです。  
正規表現を処理するということはプログラム内の同じ特徴を持つ文字を一気に変更したり削除したりできるということです。  
  
reモジュールには以下の[三つの関数](https://www.sejuku.net/blog/23232)を扱うことができます。  
  
match関数  
search関数  
findall関数  
  
match関数では指定した文字が文字列の先頭に存在するかを判定し、search関数では指定した文字一つが文字列に存在するかを判定し、fineall関数では指定した複数の文字が存在しているかを判定することができます。  
  
プログラムの書き方は以下の通りです。  
  
match関数  
```Python  
import re  
address = "123-7777 東京都千代田区"  
postCode = re.match('[0-9]{3}-[0-9]{4}' , address)  
print (postCode)  
```   
serch関数
```Python  
import re
address2 = "東京都千代田区 123-7777"
postCode = re.search('[0-9]{3}-[0-9]{4}' , address2)
print (postCode)  
```  
findall関数  
```Python
import re
address3 = "東京都千代田区 123-7777, 東京都世田谷区 567-9999"
postCodeList = re.findall('[0-9]{3}-[0-9]{4}' , address3)
if postCodeList:
    print (postCodeList)
```  

次に[math](https://www.itbook.info/network/python09.html),[random](https://www.sejuku.net/blog/20915),[statistics](https://algorithm.joho.info/programming/python/statistics-mean-median-mode-pvariance/)モジュールについて解説します。  
[mathモジュール](https://www.itbook.info/network/python09.html)はおなじみのモジュールのため関数の種類と機能のみ紹介します。  
   
|Type|Purpose|
|---|---|
|sqrt()|平方根を示す|
|floor()|切り捨ての整数を示す|
|ceil()|切り上げの整数を示す|
|trunc()|小数点以下を切り捨て|
|exp()|塁上を示す|
|log()|自然対数を示す|
|pow()|何乗を示す|
|sin(),cos(),tan()|サイン、コサイン、タンジェントを示す|
  
[randomモジュール](https://www.sejuku.net/blog/20915)ではその名の通りrandomな数字や文字列を表示してくれます。  
コードは以下の通りです。  
```Python
import random

num = random.randint(1,10)
print(num)
```  
`8`
実はrandomモジュールにも関数がいくつか存在します。上のプログラムではrandint関数を使用しました。  
  
|Type|Purpose|Example|
|---|---|---|
|random()|0.0-1.0の範囲のfloat型のランダムな値を示す|tandom.random()|
|uniform()|指定した範囲のfloat型のランダムな値を示す|random.uniform(2.0,5.0)|
|randint()|指定した範囲のint型のランダムな値を示す|random.randint(1,10)|
|choice()|リストや文字列などのシーケンス型の中から一つをランダムに示す|random.choice(mylist)|
|shuffle()|リストや文字列などシーケンス型のオブジェクトをランダムにシャッフルする|random.shuffle(mylist)|  
  
  
[statisticsモジュール](https://algorithm.joho.info/programming/python/statistics-mean-median-mode-pvariance/)では平均、中央値、最頻値、分散、標準偏差などを計算することができます。  
  
|Type|Purpose|
|---|---|
|mean()|平均を示す|
|harmonicmean()|調和平均を示す|
|median()|中央値を示す|
|mode()|最頻値を示す|
|pvariance()|母分散を示す|
|pstdev()|母集団の標準偏差を示す|
|variance()|不偏分散を示す|
|stdev()|標本標準偏差を示す|  
  
コードは以下の通りです。  
```Python
import statistics
import math

data = [1, 2, 3, 4, 5]

mean = statistics.mean(data)
print(mean) # 3


median = statistics.median(data)
print(median) # 3


median_low = statistics.median_low(data)
print(median_low) # 3

median_high = statistics.median_high(data)
print(median_high) # 3

pvariance = statistics.pvariance(data)
print(pvariance) # 2

pstdev = statistics.pstdev(data)
print(pstdev) # 1.4142135623730951

variance = statistics.variance(data)
print(variance) # 2.5

stdev = statistics.stdev(data)
print(stdev) # 1.5811388300841898
```
  
続いてurllib.requestモジュールとsmtplibモジュールについて  
  
timeモジュール

|Type|Purpose|Example|Result|
|---|---|---|---|
|sleep()|〜秒間プログラムを停止させる|time.sleep(2)|2秒止まる|

  
  
  
  
# 参考文献  
[インタプリンタとは](https://www.otsuka-shokai.co.jp/words/interpreter.html) 2019/09/22 L14-22  
[マイナス値のfloor,trunc,ceil,roundとキャストの違い](http://blog.jojo.jp/?eid=1424790) 2019/09/24 L57-60  
[クラスについて](https://eng-entrance.com/what-oop#i) 2019/09/26 L151-170  
[クラスメソッドとは](https://pg-chain.com/python-module-class-method) 2019/09/26 L151-179  
[例外とraiseとは](https://snowtree-injune.com/2018/09/14/exception/#toc34) 2019/09/25 L212-216  
[global宣言とnonlocal宣言](https://snowtree-injune.com/2018/12/13/global-nonlocal/#toc2) 2019/09/25 L223-224  
[a](https://www.sejuku.net/blog/24672) 2019/09/27 L231-240  
[a](https://python.ms/namespace/) 2019/10/01 L291-  
[a](https://python.ms/namespace/scope/#_1-ざっくり全体像)　2019/10/01 L301-  
[a](https://blog.amedama.jp/entry/2017/11/23/213233) 2019/10/02 L373-410  
[a](https://www.sejuku.net/blog/63651) 2019/10/02 L423-434  
[a](https://narito.ninja/blog/detail/71/) 2019/10/02 L449-460  
[a](https://techacademy.jp/magazine/18928) 2019/10/02 L463-473  
