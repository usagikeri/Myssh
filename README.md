# myssh

## Overview
sshの接続先の登録，削除と接続ができる．  
設定ファイルは ``~/.myssh_conf``  

## Usage
```
$chmod a+x myssh
$cp myssh /usr/local/bin/
```
mysshが実行可能になる．

### ホストの登録
```
$myssh -a
ユーザ名を入力してください．
test
ホスト名を入力してください．
127.0.0.1
説明文を入力してください．
test
```

### 登録ホストの一覧
```
$myssh -l
Number  UserName  HostName  Discription
  1     test    127.0.0.1  test
```

### ssh接続
```
$myssh
Number  USERNAME  HostName  Discription
  1     test    127.0.0.1  test
接続したい宛先の数字を入力してください．
1
```

### ホストの削除
```
$myssh -r
Number  USERNAME  HostName  Discription
  1     test    127.0.0.1  test
削除したい宛先の番号を入力してください．
1
```

### helpの表示
```
$myssh -h
Usage: myssh [option]

オプション:
  -h help
  -a add new host
  -l host list
  -r remove host

```
