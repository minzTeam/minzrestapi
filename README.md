# REST API | Minz Teambot™

### Apikey Required
You need <a href="https://api.minzteam.xyz">apikey</a> to get the response

### Example Request
Use minzrestapi.py
```python
from minzrestapi import *

api = MinzRestApi('YOUR APIKEY')
data = api.joox("Golden Hour")

api.print_result(data)
```
Use Function Request
```python
import requests, json

params = {
  "apikey": "YOUR APIKEY",
  "query": "Golden Hour"
}
api = requests.get("https://api.minzteam.xyz/joox", params=params).json()

print(api)
```
JSON Result
```json
{
    "code": 200,
    "result": {
        "audioUrl": "https://id.stream.music.joox.com/C400Z2904715120CAE.m4a?vkey=6B50675275CC3B96A307AF62A8BB124980D448B267B520A0E2838341A6F38652EE03F78A0CDA292B1837B9506661E7949D4D33415FA2E096&amp;hdnts=exp=1685745983~acl=/*~hmac=a10ada93a17b37ba812aad1a2003dfdda8d3664307c1f4387c8ade6795d4ce54&fromtag=8&guid=JOOX@WEB_OPENUDID",
        "imageUrl": "https://image.joox.com/JOOXcover/0/a49f7ab72d5918d5/1000",
        "singer": "Jvke",
        "title": "golden hour"
    }
}
```

### Full Documentation
* <a href="https://api.minzteam.xyz/">REST API</a>

### Contact For Buy Apikey
* <a href="https://line.me/ti/p/~visss.">Giusto Nur Rais</a>