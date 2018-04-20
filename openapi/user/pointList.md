---
title: OPEN API - user - pointList
---

# pointList
---

포인트 내역을 조회합니다.

## **Parameter**

다음의 URL을 통해 접근 가능합니다. 
**HTTP GET** `http://www.gamekiki.com:3000/api/v1/kiki/pointList`

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
    "isLast": "false",
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJhcHBJZCI6ImFwcF9ZTnZaZHMxRDAwMDAwIiwidXNlcklkIjoidGVzdCIsImV4cCI6MTUyNDI4NzA3NzgwOSwicmVnRGF0ZSI6IjIwMTgtMDQtMjAgMTQ6MDQ6MzcuODA3In0.UMXSiSVfEMrG7tHq0RJTj_TxHZ_aUhQ7UYopMIG40b0",
    "result": {
        "userPoint": 0,
        "pointSumInfos": [
            {
                "userId": "test",
                "sign1": "+",
                "sum(point)": 2
            }
        ],
        "pointList": [
            {
                "sign1": "+",
                "point": 1,
                "writeDate": "2018-04-19T15:58:04.000Z",
                "comments": "상품추천 클릭 완료",
                "actId": "act_CxwGaDUJ00000",
                "actname": "상품추천 클릭"
            },
            {
                "sign1": "+",
                "point": 1,
                "writeDate": "2018-04-19T15:43:36.000Z",
                "comments": "상품추천 클릭 완료",
                "actId": "act_CxwGaDUJ00000",
                "actname": "상품추천 클릭"
            },
            {
                "sign1": "+",
                "point": 1,
                "writeDate": "2018-02-07T17:27:33.000Z",
                "comments": "로그인 완료",
                "actId": "act_D93CvkiM00000",
                "actname": "로그인"
            }
        ]
    }
}
```
