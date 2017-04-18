# leaning-golang

leaning website  
[A Tour of Go](https://go-tour-jp.appspot.com/welcome/1)

#### MacOS install tutorial

```
brew install go
```

```
# インスコできない
go tool tour
```

```
# 環境変数指定なしでも以下のディレクトリがデフォ
export GOPATH=$HOME/go
```

```
go get golang.org/x/tour/gotour
```

```
cd $GOPATH/bin
./gotour
```

ローカル実行だと英語のみ...`A Tour of Goで学習をする`

#### 第1章
goでは、実行開始のプログラムにはpackage mainが必須  
Syntaxが独特。これは読みやすさを考慮した設計になっている  
importはまとめて記述する書き方がある。  
これを`factored import statement`という

Goでは、最初の文字が大文字で始まる名前は、  
外部のパッケージから参照できるエクスポート（公開）された名前( exported name )  
例えば、 Pi は math パッケージでエクスポートされる


###### basics/5
関数の宣言はfuncで始まる  
2つ以上の引数が同じ型であれば、最後に宣言した型名だけ残して他は省略できる。  
関数の戻り値は複数返す事ができる  
``naked return``と言って、戻り値に変数名をつける事でreturnに何も書かずに値を返せる
`:=`で暗黙的型変換ができる

*変数の型

* bool  
* string   
* int  int8  int16  int32  int64 uint uint8 uint16 uint32 uint64 uintptr  
* byte // uint8 の別名  
* rune // int32 の別名 // Unicode のコードポイントを表す 
* float32 float64  
* complex64 complex128  

intは32bit, 64bit環境でデータサイズが変わるためint型を推奨

* 型変換(キャスト)

キャスト構文は、`型名(値)`と記述する

定数は`const`キーワード  
使用可能な型は、文字(character)、文字列(string)、boolean、数値(numeric)のみ

https://go-tour-jp.appspot.com/basics/16


