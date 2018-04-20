---
title: OPEN API - user - profile
---

# profile
---

사용자 프로필을 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/profile`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 로그인한 사용자의 user ID  
targetUserId | test1 | Optional | 조회하고자 하는 사용자의 user ID  

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
    "result": {
        "userId": "test",
        "userName": "test",
        "userPoint": 0,
        "levelId": "1",
        "minPoint": 0,
        "nextminPoint": 101,
        "userImg": null,
        "ranking": 21,
        "achiCnt": 0,
        "compachiCnt": 0,
        "badgeInfo": [],
        "friendsCount": 0
    }
}
```
