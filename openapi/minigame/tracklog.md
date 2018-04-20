---
title: OPEN API - user - tracklog
---

# tracklog
---

사용자의 위젯과련 활동내역을 기록합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP POST** `http://www.gamekiki.com:3000/api/v1/kiki/mg/tracklog`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 로그인 User ID
eventTyp | G | Required | 활동구분1 (G:미니게임/P:상품추천/D:대시보드)
eventId | MGMAI_y588M4x6 | Required(eventTyp : G,P 인 경우) | 활동구분 ID (미니게임:mgId/상품추천:prodId)
eventChk | L | Required(eventTyp : G,P 인 경우) | 활동구분2 (L:노출/C:클릭)
todayNumb | 1 | Required(eventTyp : G,P 인 경우) | 당일 실행(노출/클릭) 누적횟수 
contNumb | 1 | Required(eventTyp : G,P 인 경우) | 연속 실행(노출/클릭) 횟수

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "userId": "test",
    "eventTyp": "G",
    "eventId": "MGMAI_y588M4x6",
    "eventChk": "L",
    "todayNumb": 1,
    "contNumb": 1
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
