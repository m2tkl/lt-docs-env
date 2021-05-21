# Code blockの拡張機能

## 行番号の表示

行番号を表示することができます。  
デフォルトでONにすることも、必要な場所だけONにすることも可能です。

``` python
def hello():
    for i in range(10):
        print('hello\n')
```

``` python linenums="1"
def hello():
    for i in range(10):
        print('hello\n')
```

## 特定の行をハイライト

行数を指定してハイライトすることができます。  

``` python linenums="1" hl_lines="2 5"
def triple_loop():
    for i in range(10):
        for j in range(10):
            for k in range(10):
                print('hello')
```
