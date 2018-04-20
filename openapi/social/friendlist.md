---
title: OPEN API - user - friendlist
---

# friendlist
---

친구 리스트를 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/friendlist`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Required | login token
userId | test | Required | 로그인 User ID
targetUserId | test | Optional | 조회하고자 하는 User ID  

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
    "result": [
        {
            "UserId": "bhksis",
            "Username": "bhksis",
            "userPoint": 38,
            "userImg": null,
            "ranking": 802,
            "levelId": "1"
        },
        {
            "UserId": "beauty7113",
            "Username": "beauty7113",
            "userPoint": 245,
            "userImg": null,
            "ranking": 44,
            "levelId": "3"
        },
        {
            "UserId": "bluesy2",
            "Username": "bluesy2",
            "userPoint": 112,
            "userImg": null,
            "ranking": 410,
            "levelId": "2"
        },
        {
            "UserId": "berith79",
            "Username": "berith79",
            "userPoint": 132,
            "userImg": null,
            "ranking": 330,
            "levelId": "2"
        },
        {
            "UserId": "bnw3000",
            "Username": "bnw3000",
            "userPoint": 0,
            "userImg": null,
            "ranking": 5325,
            "levelId": "1"
        },
        {
            "UserId": "frdTest02",
            "Username": "frdTest02",
            "userPoint": 1,
            "userImg": null,
            "ranking": 3328,
            "levelId": "1"
        },
        {
            "UserId": "inword311",
            "Username": "inword311",
            "userPoint": 107,
            "userImg": "../data/userImg/app_Bx8BoU1g00000/1460623827974_IMG_20121012_101619.jpg",
            "ranking": 434,
            "levelId": "2"
        },
        {
            "UserId": "cns6853",
            "Username": "cns6853",
            "userPoint": 110,
            "userImg": null,
            "ranking": 425,
            "levelId": "2"
        },
        {
            "UserId": "ks",
            "Username": "ks",
            "userPoint": 61,
            "userImg": "../data/userImg/app_Bx8BoU1g00000/1486430533420_androidmarker.png",
            "ranking": 652,
            "levelId": "1"
        },
        {
            "UserId": "test06",
            "Username": "test06",
            "userPoint": 0,
            "userImg": null,
            "ranking": 5325,
            "levelId": "1"
        },
        {
            "UserId": "kimyhzz",
            "Username": "kimyhzz",
            "userPoint": 212,
            "userImg": null,
            "ranking": 98,
            "levelId": "3"
        },
        {
            "UserId": "frdTest01",
            "Username": "frdTes31",
            "userPoint": 27,
            "userImg": "../data/userImg/app_Bx8BoU1g00000/1467772498767_20141109_171422.jpg",
            "ranking": 935,
            "levelId": "1"
        },
        {
            "UserId": "test11",
            "Username": "test11",
            "userPoint": 0,
            "userImg": null,
            "ranking": 5325,
            "levelId": "1"
        },
        {
            "UserId": "test115",
            "Username": "test115",
            "userPoint": 0,
            "userImg": null,
            "ranking": 5325,
            "levelId": "1"
        },
        {
            "UserId": "jo3419",
            "Username": "jo3419",
            "userPoint": 24,
            "userImg": null,
            "ranking": 979,
            "levelId": "1"
        }
    ]
}
```
