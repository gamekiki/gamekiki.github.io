---
title: OPEN API - user - toplist
---

# toplist
---

상위랭킹을 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/toplist`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Optional | login token
isFriend | N | Optional | 친구 랭킹정보 조회 여부. 'Y'인 경우 친구 랭킹 조회  
pageNo | 1 | Optional | 조회 페이지 정보. 페이지당 20건 조회
pageSize | 20 | Optional | 한페이지에 조회할 리스트 갯수
userId | test | Optional | 로그인 User ID

## **Example**

보내는 메시지는 아래와 같습니다.

```json
{
    "appId": "app_Bx8BoU1g00000"
}
```

## **Response**

받는 값은 아래와 같습니다.

```json
{
    "updatedToken": "N",
    "isLast": "false",
    "result": {
        "myRankInfo": [
            {
                "ranking": 21,
                "userId": "test",
                "username": "test1234",
                "userImg": "null",
                "UserPoint": 0,
                "levelId": "1"
            }
        ],
        "rankList": [
            {
                "ranking": 1,
                "userId": "test100",
                "username": "test100",
                "userImg": null,
                "UserPoint": 6,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 2,
                "userId": "ratm0424",
                "username": "ratm0424",
                "userImg": null,
                "UserPoint": 5,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 3,
                "userId": "cascade",
                "username": "cascade",
                "userImg": null,
                "UserPoint": 4,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 3,
                "userId": "shleetest04",
                "username": "shleetest04",
                "userImg": null,
                "UserPoint": 4,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 3,
                "userId": "shleetest09",
                "username": "shleetest09",
                "userImg": null,
                "UserPoint": 4,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 3,
                "userId": "yueum88",
                "username": "yueum88",
                "userImg": null,
                "UserPoint": 4,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 7,
                "userId": "shleetest01",
                "username": "shleetest01",
                "userImg": null,
                "UserPoint": 3,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 7,
                "userId": "bookoa",
                "username": "bookoa",
                "userImg": null,
                "UserPoint": 3,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 7,
                "userId": "bookzzin",
                "username": "bookzzin",
                "userImg": null,
                "UserPoint": 3,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 10,
                "userId": "shleetest06",
                "username": "shleetest06",
                "userImg": null,
                "UserPoint": 2,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 10,
                "userId": "inword",
                "username": "inword",
                "userImg": null,
                "UserPoint": 2,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 10,
                "userId": "shleetest02",
                "username": "shleetest02",
                "userImg": null,
                "UserPoint": 2,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 10,
                "userId": "shleetest07",
                "username": "shleetest07",
                "userImg": null,
                "UserPoint": 2,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 10,
                "userId": "oingoing",
                "username": "oingoing",
                "userImg": null,
                "UserPoint": 2,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 10,
                "userId": "shleetest03",
                "username": "shleetest03",
                "userImg": null,
                "UserPoint": 2,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 10,
                "userId": "shleetest05",
                "username": "shleetest05",
                "userImg": null,
                "UserPoint": 2,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 17,
                "userId": "shleetest10",
                "username": "shleetest10",
                "userImg": null,
                "UserPoint": 1,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 17,
                "userId": "shleetest08",
                "username": "shleetest08",
                "userImg": null,
                "UserPoint": 1,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 17,
                "userId": "ysh111",
                "username": "ysh111",
                "userImg": null,
                "UserPoint": 1,
                "levelId": "1",
                "friendFlag": null
            },
            {
                "ranking": 17,
                "userId": "rururu20",
                "username": "rururu20",
                "userImg": null,
                "UserPoint": 1,
                "levelId": "1",
                "friendFlag": null
            }
        ]
    }
}
```