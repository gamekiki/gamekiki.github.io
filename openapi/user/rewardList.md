---
title: OPEN API - user - rewardList
---

# rewardList
---

리워드 정보를 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/rewardList`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Optional | login token
userId | test | Optional | 로그인 User ID

## **Example**

보내는 메시지는 아래와 같습니다.

```javascript
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test"
}
```

## **Response**

받는 값은 아래와 같습니다.

```javascript
{
    "updatedToken": "N",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "result": [
        {
            "actName": "로그인",
            "actDesc": "",
            "rewKind": "P",
            "rewardValue": "1",
            "restricted": "1",
            "badgeImg": null
        },
        {
            "actName": "상품추천 클릭",
            "actDesc": "",
            "rewKind": "P",
            "rewardValue": "1",
            "restricted": "5",
            "badgeImg": null
        },
        {
            "actName": "룰렛 실행",
            "actDesc": "",
            "rewKind": "P",
            "rewardValue": "1",
            "restricted": "1",
            "badgeImg": null
        }
    ]
}
```