---
title: OPEN API - user - login
---

# login
---

사용자 로그인을 처리합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP POST** `http://www.gamekiki.com:3000/login`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
secretKey | 456951cb56f161215d6147083b03970c0f..... | Required | Application Secret Key (CMS에서 확인 가능)
userId | test | Required | 로그인한 사용자의 user ID
loginType | P | Optional | 유입경로, A:android / I:iOS / P:PC / E:eMail / F:facebook/ K:kakao

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "secretKey": "456951cb56f161215d6147083b03970c0f.....",
    "userId": "test"
}
```

## **Response**

받는 값은 아래와 같습니다.

```json
{
    "message": "succeed to login.",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey....."
}
```
