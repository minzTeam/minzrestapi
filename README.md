# REST API | Minz Teambot™

### APIKEY REQUIRED
You need <a href="https://api.minzteam.xyz">apikey</a> to get the response

### EXAMPLE REQUEST
Use minzrestapi.py
```python
from minzrestapi import *

api = MinzRestApi('YOUR APIKEY')
data = api.joox("Golden Hour")

api.print_result(data)
```
Python Language
```python
import requests, json

params = {
  "apikey": "YOUR APIKEY",
  "query": "Golden Hour"
}
api = requests.get("https://api.minzteam.xyz/joox", params=params).json()

print(api)
```
Google Language
```go
package main

import ("net/http"; "net/url"; "fmt"; "encoding/json")

func main() {
    baseURL := "http://api.minzteam.xyz"
    resource := "/joox"
    params := url.Values{}
    params.Add("apikey", "YOUR_APIKEY")
    params.Add("query", "Golden Hour")

    u, _ := url.ParseRequestURI(baseURL)
    u.Path = resource
    u.RawQuery = params.Encode()
    urlStr := fmt.Sprintf("%v", u)

    r, _ := http.Get(urlStr)
    defer r.Body.Close()
}
```
JavaScript Language
```javascript
fetch('https://api.minzteam.xyz/joox?query=Golden%20Hour&apikey=YOUR_APIKEY')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error(error));
```
PHP Language
```php
$ch = curl_init();

curl_setopt($ch, CURLOPT_URL, 'https://api.minzteam.xyz/joox?query=Golden%20Hour&apikey=YOUR_APIKEY');
curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
curl_setopt($ch, CURLOPT_CUSTOMREQUEST, 'GET');

$result = curl_exec($ch);
if (curl_errno($ch)) {
    echo 'Error:' . curl_error($ch);
}
curl_close($ch);
```
Shell Language
```shell
curl "https://api.minzteam.xyz/joox?query=Golden%20Hour&apikey=YOUR_APIKEY" \
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

### FULL DOCUMENTATION
<a href="https://api.minzteam.xyz/">REST API</a>

### CONTACT US
<a href="https://line.me/ti/p/~visss.">CREATOR</a>

### SUPPORTED BY
* Alm. ZeroCool
* Phantom Coder
* Superline Project
* Vnyll Teambot
* Talk Exception
