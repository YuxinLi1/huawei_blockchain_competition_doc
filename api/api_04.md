# 学习者接口

- 系统推荐

  | Description            | HTTP Mapping                    | HTTP RequestBody | HTTP ResponseBody |
  | ---------------------- | ------------------------------- | ---------------- | ----------------- |
  | 返回系统推荐的一些课程 | GET /learner/{learner_id}/items | N/A              | {"items": []}     |




- 课程详情

  | Description            | HTTP Mapping                              | HTTP RequestBody | HTTP ResponseBody   |
  | ---------------------- | ----------------------------------------- | ---------------- | ------------------- |
  | 返回指定课程的详细信息 | GET /learner/{learner_id}/items/{item_id} | N/A              | {"item_detail": {}} |




- 个人课程

  | Description                | HTTP Mapping                       | HTTP RequestBody | HTTP ResponseBody |
  | -------------------------- | ---------------------------------- | ---------------- | ----------------- |
  | 返回学习者所参与的所有课程 | GET /learner/{learner_id}/my_items | N/A              | {"my_items": []}  |




- 个人课程详情

  | Description                        | HTTP Mapping                                 | HTTP RequestBody | HTTP ResponseBody   |
  | ---------------------------------- | -------------------------------------------- | ---------------- | ------------------- |
  | 返回学习者参与的某门课程的详细信息 | GET /learner/{learner_id}/my_items/{item_id} | N/A              | {"item_detail": {}} |




- 个人证书

  | Description                  | HTTP Mapping                    | HTTP RequestBody | HTTP ResponseBody |
  | ---------------------------- | ------------------------------- | ---------------- | ----------------- |
  | 返回学习者所认证的成果即证书 | GET /learner/{learner_id}/certs | N/A              | {"certs": []}     |




- 更新学习状态

  | Description                            | HTTP Mapping                                      | HTTP RequestBody | HTTP ResponseBody |
  | -------------------------------------- | ------------------------------------------------- | ---------------- | ----------------- |
  | 更新学习者某门课程的状态，如提交认证等 | POST /learner/{learner_id}/items-update/{item_id} | {"option": ""}   | Empty             |



> 以上“课程”包括课程、项目、竞赛、实习、活动等各种类型