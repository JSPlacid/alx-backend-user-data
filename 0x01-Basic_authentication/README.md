# Basic authentication
![](https://camo.githubusercontent.com/dbee9377978d25748c641f11f50faedba44ee215b2e23d8abd7ac04619269f0d/68747470733a2f2f646f63732e6f7261636c652e636f6d2f63642f4531393837392d30312f3831392d333636392f696d616765732f73656375726974792d68747470426173696341757468656e7469636174696f6e2e676966)

### Resources
**Read or watch:**

- [REST API Authentication Mechanisms](https://intranet.alxswe.com/rltoken/ssg5umgsMk5jKM8WRHk2Ug)
- [Base64 in Python](https://intranet.alxswe.com/rltoken/RpaPRyKx1rdHgRSUyuPfeg)
- [HTTP header Authorization](https://intranet.alxswe.com/rltoken/WlARq8tQPUGQq5VphLKM4w)
- [Flask](https://intranet.alxswe.com/rltoken/HG5WXgSja5kMa29fbMd9Aw)
- [Base64 - concept](https://intranet.alxswe.com/rltoken/br6Rp4iMaOce6EAC-JQnOw)

### learning objectives

- What authentication means
- What Base64 is
- How to encode a string in Base64
- What Basic authentication means
- How to send the Authorization header

#### simple API
simple http API for playing with user auth model
#### Files
**models*/*
- base.py: base of all models of the API - handle serialization to file
- user.py: user model

#### api/v1
- app.py: entry point of the API
- views/index.py: basic endpoints of the API: /status and /stats
- views/users.py: all users endpoints

#### setup
```$ pip3 freeze > requirementts.txt```

#### Run
```$ API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app```

#### Routes 
- GET /api/v1/status: returns the status of the API
- GET /api/v1/stats: returns some stats of the API
- GET /api/v1/users: returns the list of users
- GET /api/v1/users/🆔 returns an user based on the ID
- DELETE /api/v1/users/🆔 deletes an user based on the ID
- POST /api/v1/users: creates a new user (JSON parameters: email, password, last_name (optional) and first_name (optional))
- PUT /api/v1/users/🆔 updates an user based on the ID (JSON parameters: last_name and first_name)
