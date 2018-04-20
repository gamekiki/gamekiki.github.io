---
title: OPEN API - user - userLevel
---

# userLevel
---

사용자 레벨정보를 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/userLevel`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
targetUserId | test | Required | 조회하고자 하는 User ID

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "targetUserId": "test"
}
```

## **Response**

받는 값은 아래와 같습니다.

```json
{
    "updatedToken": "N",
    "result": [
        {
            "userId": "test",
            "userName": "test1234",
            "userPoint": 2,
            "levelId": "1"
        }
    ]
}
```
