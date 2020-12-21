# # pyenv, pyenv-virtualenv の環境構築備忘録

## 1. 基本
### 1.1. pyenv とは
&nbsp;**1 つのマシンに複数のバージョンの Python をインストールし、それらを切り替えて使うための仕組み**&nbsp;のこと。

例:「プロジェクトA では v3.8.5 を使うが、メンテナンスモードに入っている古いプロジェクトBでは v3.6.9 を使わなければならない」場合<br/>
- 一々 Python をインストールし直していたら面倒。
- そんな時に pyenv を使えば複数のバージョンの Python をインストールし、それらを切り替えて使うことができる。


---
### 1.2. pyenv-virtualenv とは
&nbsp;**virtualenv を pyenv の中でイイ感じに使えるようにした仕組み**&nbsp;のこと。<br/>

**● virtualenv とは:**<br/>
&nbsp;**あるバージョンの Python 環境を複数持つための仕組み**&nbsp;のこと [1]。<br/>
&emsp; --> これによって「Python はシステム全体で依存ライブラリを 1 セットしか保持できない」という問題を解決できる。<br/>

例:「プロジェクトA は requests と pytorch に依存していて、プロジェクトB は pandas と numpy に依存している」場合<br/>
プロジェクトA も B も同じバージョンの Python で動く場合、1 つの Python バージョンに対し、双方の依存ライブラリをインストールしなければならない。<br/>
&emsp; --> この場合、ライブラリ同士の衝突が起きてしまう可能性がある。<br/>

上記を避けるために、プロジェクトA 用の v3.8.5 と、プロジェクトB 用の v3.8.5を作る必要がある。これをしてくれるのが virtualenv。<br/>

---
## 2. 構築手順
```
comming soon
```


---
### 参考資料
[1] Virtualenv documentation
https://virtualenv.pypa.io/en/latest/
```
virtualenv is a tool to create isolated Python environments.
```
