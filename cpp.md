## set
    - 要素に重複がない連想コンテナ

## char string
- charは文字型。単一の文字の表現。
- stringは文字列を扱う型。0個以上任意個数の char の並び表現。


## シーケンスコンテナと連想コンテナ
    - 要素の値に関係なく、追加されたタイミングなどによって要素の位置が決定されます。
    - 連想コンテナでは何らかの基準に従って要素がソートされています。setとmapは連想コンテナに分別されます。
    - 要素がソートされていることによって、連想コンテナは高速な二分探索を利用できるという利点があります。
[参照](https://programgenjin.hatenablog.com/entry/2019/03/02/141225)


## 御作法
- #include <bits/stdc++.h>はC++の機能をすべて読み込むための命令
cout endl; だけであれば #include <iostream> で足りる

- using namespace std; プログラムを短く書くための機能   
    #includeで読み込んだC++の機能を利用するためには、通常はstd::coutやstd::endlのようにstd::をはじめに付ける必要があります。
using namespace std;を利用すると、このstd::を省略して書くことができます。