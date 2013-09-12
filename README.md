rehichao
========
redis生成管理key

Installation
=====

requires: **intstr** **redis**
``$ pip install rehichao``

Getting Started
=====

```python
from rehichao import RedisKey
redis_config = ("192.168.1.220", 10001, 10)
redis_key = RedisKey(redis_config)
redis, test_key = redis_key.TestKey()
uid = 12345
redis.hincrby(test_key, uid)
```
