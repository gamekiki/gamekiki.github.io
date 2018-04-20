---
title: OPEN API - user - reqfriendlist
---

# reqfriendlist
---

친구요청 리스트를 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/reqfriendlist`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 로그인 User ID

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test"
}
```

## **Response**

받는 값은 아래와 같습니다.

```json
{
    "updatedToken": "N",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "result": [
        {
            "userId": "test1",
            "userName": "test1",
            "userPoint": 111,
            "badgeimg": "./images/badge01.jpg",
            "userImg": "./images/test1.jpg",
            "ranking": 11,
            "levelId": 1
        },
        {
            "userId": "test2",
            "userName": "test2",
            "userPoint": 222,
            "badgeimg": "./images/badge02.jpg",
            "userImg": "./images/test2.jpg",
            "ranking": 22,
            "levelId": 2
        },
        {
            "userId": "test3",
            "userName": "test3",
            "userPoint": 333,
            "badgeimg": "./images/badge03.jpg",
            "userImg": "./images/test3.jpg",
            "ranking": 33,
            "levelId": 3
        }
    ]
}
```
