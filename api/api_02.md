# 公用接口

- 主页

  | Description | HTTP Mapping | HTTP RequestBody | HTTP ResponseBody |
  | ----------- | ------------ | ---------------- | ----------------- |
  | 返回主页    | GET /        | N/A              | html              |



- 查询验证证书

  | Description                                        | HTTP Mapping      | HTTP RequestBody | HTTP ResponseBody             |
  | -------------------------------------------------- | ----------------- | ---------------- | ----------------------------- |
  | 根据输入的Hash值查询并验证该Hash对应的所有证书信息 | POST /query_certs | {"hash": ""}     | {"key": "certs", "value": []} |

  