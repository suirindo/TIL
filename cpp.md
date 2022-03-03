## set
    - 要素に重複がない連想コンテナ

## char string
- charは文字型。単一の文字の表現。
- stringは文字列を扱う型。0個以上任意個数の char の並び表現。

## ２次元配列
- vector<vector<要素の型>> 変数名(要素数1, vector<要素の型>(要素数2, 初期値))
```C++
  // int型の2次元配列(3×4要素の)の宣言
  vector<vector<int>> data(3, vector<int>(4));

```

## map
- std::map とは C++ で標準に使用できる便利な連想配列クラス

```C++
std::map<std::string, int>
```
テンプレート第一引数のstd::stringがkey
テンプレート第二引数のintがvalue
である.
mapはkeyからvalueを検索するのが得意である.
mapを利用する理由の殆どはその高速な値の検索にあると言って良い.

参照：[std::mapまとめ](https://qiita.com/_EnumHack/items/f462042ec99a31881a81)
2022.3.3 理解がいまいちである。


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