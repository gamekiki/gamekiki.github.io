---
title: OPEN API - user - feed
---

# feed
---

최근 활동내역을 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/feed`

Parameter | Example | Required | Description
---|---|---|---
appId | app_Bx8BoU1g00000 | Required | Application ID (CMS에서 확인 가능)
token | eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ey..... | Optional | login token
isFriend | N | Optional | 친구 활동내역 조회 여부. 'Y'인 경우 친구 활동내역만 조회  
pageNo | 1 | Optional | 조회 페이지 정보. 페이지당 20건 조회
isMine | N | Optional | 내 활동내역만 조회 여부. 'Y'인 경우 내 활동내역만 조회 

## **Example**

보내는 메시지는 아래와 같습니다.

```javascript
{
    "appId": "app_Bx8BoU1g00000"
}
```

## **Response**

받는 값은 아래와 같습니다.

```javascript
{
    "updatedToken": "N",
    "isLast": "false",
    "result": [
        {
            "recordSerno": 363606,
            "UserId": "shleetest09",
            "Username": "shleetest09",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T19:11:24.000Z"
        },
        {
            "recordSerno": 363605,
            "UserId": "shleetest01",
            "Username": "shleetest01",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T19:11:10.000Z"
        },
        {
            "recordSerno": 363604,
            "UserId": "shleetest09",
            "Username": "shleetest09",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T19:06:11.000Z"
        },
        {
            "recordSerno": 363603,
            "UserId": "shleetest09",
            "Username": "shleetest09",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T18:51:43.000Z"
        },
        {
            "recordSerno": 363602,
            "UserId": "yueum88",
            "Username": "yueum88",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T18:50:16.000Z"
        },
        {
            "recordSerno": 363601,
            "UserId": "shleetest09",
            "Username": "shleetest09",
            "userImg": null,
            "actName": "룰렛 실행",
            "regiYHS": "2018-04-18T18:27:59.000Z"
        },
        {
            "recordSerno": 363600,
            "UserId": "shleetest09",
            "Username": "shleetest09",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T18:27:50.000Z"
        },
        {
            "recordSerno": 363599,
            "UserId": "shleetest09",
            "Username": "shleetest09",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T18:01:00.000Z"
        },
        {
            "recordSerno": 363598,
            "UserId": "yueum88",
            "Username": "yueum88",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T18:00:34.000Z"
        },
        {
            "recordSerno": 363597,
            "UserId": "shleetest08",
            "Username": "shleetest08",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T17:39:31.000Z"
        },
        {
            "recordSerno": 363596,
            "UserId": "yueum88",
            "Username": "yueum88",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T17:12:33.000Z"
        },
        {
            "recordSerno": 363595,
            "UserId": "yueum88",
            "Username": "yueum88",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T17:08:19.000Z"
        },
        {
            "recordSerno": 363594,
            "UserId": "shleetest06",
            "Username": "shleetest06",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T17:08:07.000Z"
        },
        {
            "recordSerno": 363593,
            "UserId": "test100",
            "Username": "test100",
            "userImg": null,
            "actName": "룰렛 실행",
            "regiYHS": "2018-04-18T17:06:32.000Z"
        },
        {
            "recordSerno": 363592,
            "UserId": "test100",
            "Username": "test100",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T17:06:23.000Z"
        },
        {
            "recordSerno": 363591,
            "UserId": "test100",
            "Username": "test100",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T17:06:23.000Z"
        },
        {
            "recordSerno": 363590,
            "UserId": "yueum88",
            "Username": "yueum88",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T16:59:25.000Z"
        },
        {
            "recordSerno": 363589,
            "UserId": "yueum88",
            "Username": "yueum88",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T16:56:58.000Z"
        },
        {
            "recordSerno": 363588,
            "UserId": "yueum88",
            "Username": "yueum88",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T16:56:31.000Z"
        },
        {
            "recordSerno": 363587,
            "UserId": "shleetest08",
            "Username": "shleetest08",
            "userImg": null,
            "actName": "로그인",
            "regiYHS": "2018-04-18T16:56:15.000Z"
        }
    ]
}
```
