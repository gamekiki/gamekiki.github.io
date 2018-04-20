---
title: OPEN API - user - srcfriend
---

# srcfriend
---

username으로 사용자를 검색합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/srcfriend`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 로그인 User ID
kWord | user | Required | 검색 키워드

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test",
    "kWord": "user"
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
            "userId": "user0003",
            "Username": "user0003",
            "userPoint": 0,
            "badgeimg": "",
            "userImg": null,
            "ranking": 5325,
            "levelId": "1",
            "friendFlag": null
        },
        {
            "userId": "user001",
            "Username": "user001",
            "userPoint": 45,
            "badgeimg": "bag_MiZiC8Ya00000_badge04.png|| badge04.png",
            "userImg": null,
            "ranking": 755,
            "levelId": "1",
            "friendFlag": null
        },
        {
            "userId": "user01",
            "Username": "user01",
            "userPoint": 3,
            "badgeimg": null,
            "userImg": null,
            "ranking": 2431,
            "levelId": "1",
            "friendFlag": null
        }
    ]
}
```
