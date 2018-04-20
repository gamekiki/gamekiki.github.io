---
title: OPEN API - user - sproduct
---

# sproduct
---

추천상품 정보를 추가합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP POST** `http://www.gamekiki.com:3000/api/v1/kiki/gd/sproduct`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
prodId | prod0001 | Required | 추천상품 ID
userId | test | Required | 로그인 User ID
kword | history | Required | 추천상품 관련 키워드
prodImgUrl | ./images/history.jpg | Required | 상품썸네일 URL
prodUrl | http://www.google.com | Required | 상품상세보기 URL
prodName | 역사가 중요하다 | Required | 상품명
prodPrice | 10000 | Required | 상품가격
prodQty | 10 | Optional | 상품수량(기본값:1)

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test",
    "prodId": "prod0001",
    "kword": "history",
    "prodImgUrl": "./images/history.jpg",
    "prodUrl": "http://www.google.com",
    "prodName": "역사가 중요하다",
    "prodPrice": 10000
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
