---
title: OPEN API - user - updateProfile
---

# updateProfile
---

사용자 프로필을 수정합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP POST** `http://www.gamekiki.com:3000/api/v1/kiki/updateProfile`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 수정하려고 하는 사용자의 user ID  
userName | test123 | Optional | 수정하려고 하는 user name
userImg | ./images/profile.jpg | Optional | 수정하려고 하는 user profile image  

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test",
    "userName": "test123",
    "userImg": "./images/profile.jpg"
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
