---
title: OPEN API - user - sugfriend
---

# sugfriend
---

추천 친구를 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/sugfriend`

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
    "result": [
        {
            "UserId": "cys5151",
            "Username": "cys5151",
            "userPoint": 217,
            "userImg": null,
            "ranking": 88,
            "levelId": "3"
        },
        {
            "UserId": "jhy4726",
            "Username": "jhy4726",
            "userPoint": 7,
            "userImg": null,
            "ranking": 1623,
            "levelId": "1"
        },
        {
            "UserId": "freedom_0824",
            "Username": "freedom_0824",
            "userPoint": 97,
            "userImg": null,
            "ranking": 484,
            "levelId": "1"
        },
        {
            "UserId": "dahong61",
            "Username": "dahong61",
            "userPoint": 53,
            "userImg": null,
            "ranking": 705,
            "levelId": "1"
        },
        {
            "UserId": "hoodae",
            "Username": "hoodae",
            "userPoint": 12,
            "userImg": null,
            "ranking": 1258,
            "levelId": "1"
        },
        {
            "UserId": "dongtan76",
            "Username": "dongtan76",
            "userPoint": 23,
            "userImg": null,
            "ranking": 998,
            "levelId": "1"
        },
        {
            "UserId": "tbyeong02",
            "Username": "tbyeong02",
            "userPoint": 12,
            "userImg": null,
            "ranking": 1258,
            "levelId": "1"
        },
        {
            "UserId": "oms7919",
            "Username": "oms7919",
            "userPoint": 92,
            "userImg": null,
            "ranking": 507,
            "levelId": "1"
        },
        {
            "UserId": "teasik-59",
            "Username": "teasik-59",
            "userPoint": 5,
            "userImg": null,
            "ranking": 1905,
            "levelId": "1"
        },
        {
            "UserId": "sengme1004",
            "Username": "sengme1004",
            "userPoint": 13,
            "userImg": null,
            "ranking": 1219,
            "levelId": "1"
        },
        {
            "UserId": "ley621101",
            "Username": "ley621101",
            "userPoint": 219,
            "userImg": null,
            "ranking": 83,
            "levelId": "3"
        },
        {
            "UserId": "dbstnwl1013",
            "Username": "dbstnwl1013",
            "userPoint": 3,
            "userImg": null,
            "ranking": 2431,
            "levelId": "1"
        },
        {
            "UserId": "haebin0506",
            "Username": "haebin0506",
            "userPoint": 5,
            "userImg": null,
            "ranking": 1905,
            "levelId": "1"
        },
        {
            "UserId": "mc0931",
            "Username": "mc0931",
            "userPoint": 30,
            "userImg": null,
            "ranking": 891,
            "levelId": "1"
        },
        {
            "UserId": "eylee2016",
            "Username": "eylee2016",
            "userPoint": 7,
            "userImg": null,
            "ranking": 1623,
            "levelId": "1"
        },
        {
            "UserId": "thakd202",
            "Username": "thakd202",
            "userPoint": 60,
            "userImg": null,
            "ranking": 659,
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
            "UserId": "kojypaul",
            "Username": "kojypaul",
            "userPoint": 187,
            "userImg": null,
            "ranking": 155,
            "levelId": "2"
        },
        {
            "UserId": "in2267",
            "Username": "in2267",
            "userPoint": 205,
            "userImg": null,
            "ranking": 114,
            "levelId": "3"
        },
        {
            "UserId": "ajw515",
            "Username": "ajw515",
            "userPoint": 9,
            "userImg": null,
            "ranking": 1432,
            "levelId": "1"
        }
    ]
}
```
