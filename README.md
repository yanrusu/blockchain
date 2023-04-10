# Are you looking for the source code for my book?

Please find it here: https://github.com/dvf/blockchain-book

The book is available on Amazon: https://www.amazon.com/Learn-Blockchain-Building-Understanding-Cryptocurrencies/dp/1484251709

# Learn Blockchains by Building One

[![Build Status](https://travis-ci.org/dvf/blockchain.svg?branch=master)](https://travis-ci.org/dvf/blockchain)

This is the source code for my post on [Building a Blockchain](https://medium.com/p/117428612f46). 

## Installation

1. Make sure [Python 3.6+](https://www.python.org/downloads/) is installed. 
2. Install [pipenv](https://github.com/kennethreitz/pipenv). 

```
$ pip install pipenv 
```
3. Install requirements  
```
$ pipenv install 
``` 

4. Run the server:
    * `$ pipenv run python blockchain.py` 
    * `$ pipenv run python blockchain.py -p 5001`
    * `$ pipenv run python blockchain.py --port 5002`
    
## 功能
### 觀看區塊鏈狀態
http://127.0.0.1:5000/chain

5000端口節點 http://127.0.0.1:5000/chain 上可以看到鏈上的區塊
### 產生新區塊
http://127.0.0.1:5000/mine

5000端口節點並產生新的區塊 http://127.0.0.1:5000/mine
### 產生新交易







