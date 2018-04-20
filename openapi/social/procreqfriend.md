---
title: OPEN API - user - procreqfriend
---

# procreqfriend
---

친구요청에 대해 수락/거절 합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP POST** `http://www.gamekiki.com:3000/api/v1/kiki/procreqfriend`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 로그인 User ID
friendUserId | user | Required | 친구요청 User ID
acceptYN | Y | Required | 수락여부 (Y:수락/N:거부)  

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test",
    "friendUserId": "user",
    "acceptYN": "Y"
}
```

## **Response**

받는 값은 아래와 같습니다.

```json
{
    "updatedToken": "N",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "result": "success"
}
```
