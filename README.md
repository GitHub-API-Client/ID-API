# IP-API by [@D4RKH0R1Z0N](https://github.com/D4RKH0R1Z0N)

## From Project Hexagon by [@D4RKH0R1Z0N](https://github.com/D4RKH0R1Z0N)

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

```
  app.py --> main.py --> GitHub-API --> Stored in GitHub
```

### Create your token by going to Setting's > Developer settings > Personal Access Token > Generate New Token
#### Set never expire, click repo all permissions then copy paste to main.py

#### app.py is not available in this repo and is owned by [D4RKH0R1Z0N](https://github.com/D4RKH0R1Z0N) and its not important at all in ID-API (IP-API)
#### ID-API was a typo I meant to type IP-API and Decided to go with it and continue 😓
