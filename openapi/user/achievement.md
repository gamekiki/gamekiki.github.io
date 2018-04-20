---
title: OPEN API - user - achievement
---

# achievement
---

업적정보를 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/achievement`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 로그인 User ID
pageNo | 1 | Optional | 조회 페이지 정보. 페이지당 20건 조회
pageSize | 20 | Optional | 한페이지에 조회할 리스트 갯수

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
    "isLast": "true",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey.....",
    "result": [
        {
            "achiId": "achi_gTlP7Ur100000",
            "appId": "app_3O5oylF200000",
            "achiName": "테스트2",
            "badgeImg": "bag_UNAFXFQl00000_badge_reading_B.png|| badge_reading_B.png",
            "tCount": 5,
            "cCount": 0
        }
    ]
}
```
