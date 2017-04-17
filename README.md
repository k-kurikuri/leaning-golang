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



