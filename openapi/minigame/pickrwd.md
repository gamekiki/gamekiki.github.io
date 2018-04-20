---
title: OPEN API - user - pickrwd
---

# pickrwd
---

미니게임 실행 당첨정보를 확인합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP POST** `http://www.gamekiki.com:3000/api/v1/kiki/mg/pickrwd`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
mgId | MGMAI_y588M4x6 | Required | 미니게임 ID
userId | test | Required | 로그인 User ID

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test",
    "mgId": "MGMAI_y588M4x6"
}
```

## **Response**

받는 값은 아래와 같습니다.

```json
{
    "updatedToken": "N",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "result": {
        "rwdId": "MGSUB_U5y3e3f1",
        "rwdName": "꽝"
    }
}
```
