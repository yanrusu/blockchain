
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

5000端口節點上可以看到鏈上的區塊

### 產生新區塊
http://127.0.0.1:5000/mine

5000端口節點並產生新的區塊

### 產生新交易
```
curl http://127.0.0.1:5000/transactions/new -X POST -H "Content-Type: application/json" -d 

'{
    "sender": "d4ee26eee15148ee92c6cd394edd974e",
    "recipient": "someone-other-address",
    "amount": 5
}'
```

### 註冊新節點
先開起新節點，再進行註冊
```
curl http://127.0.0.1:5000/nodes/register -X POST -H "Content-Type: application/json" -d '{"nodes": ["http://127.0.0.1:5001"]}'
```

### 同步節點
同兩節點的狀態

http://127.0.0.1:5000/nodes/resolve










