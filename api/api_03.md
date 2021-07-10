# 注册登录接口

- 登录

  | Description | HTTP Mapping | HTTP RequestBody          | HTTP ResponseBody |
  | ----------- | ------------ | ------------------------- | ----------------- |
  | 用户登录    | POST /login  | {"uid": "", "passwd": ""} | {"uid": ""}       |




- 登出

  | Description | HTTP Mapping | HTTP RequestBody | HTTP ResponseBody |
  | ----------- | ------------ | ---------------- | ----------------- |
  | 用户登出    | GET /logout  | N/A              | Empty             |




- 注册

  | Description | HTTP Mapping   | HTTP RequestBody                      | HTTP ResponseBody |
  | ----------- | -------------- | ------------------------------------- | ----------------- |
  | 注册用户    | POST /register | {"uid": "", "name": "", "passwd": ""} | {"uid" : ""}      |
