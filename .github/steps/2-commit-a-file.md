```python
import hashlib

api_key = "api_BF4nb5rv09L3JoukcEavoSavQfoCioY8"
ip_address = "187.250.219.226"
user_agent = "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Mobile Safari/537.36"
timestamp = "2023-11-08 12:48:08"

data = api_key + ip_address + user_agent + timestamp
hash_value = hashlib.sha256(data.encode()).hexdigest()
tracker_code = hash_value[:8]

print("Tracker Code:", tracker_code)
```