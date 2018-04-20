---
title: OPEN API - user - sugprod
---

# sugprod
---

사용자에게 추천할 상품을 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/gd/sugprod`

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
    "result": {
        "prodId": "prodId0010",
        "prodImgUrl": "https://i.pinimg.com/564x/a6/f6/0c/a6f60cb46785e59b40599387c7b84fb5.jpg",
        "prodUrl": "http://www.naver.com",
        "prodName": "상품10",
        "prodPrice": 10000
    }
}
```
