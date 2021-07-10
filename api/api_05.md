# 组织者接口

- 组织者课程项目

  | Description              | HTTP Mapping            | HTTP RequestBody | HTTP ResponseBody |
  | ------------------------ | ----------------------- | ---------------- | ----------------- |
  | 返回该组织发布的所有课程 | GET /org/{org_id}/items | N/A              | {"item": []}      |




- 组织者课程详情

  | Description                                            | HTTP Mapping                      | HTTP RequestBody | HTTP ResponseBody   |
  | ------------------------------------------------------ | --------------------------------- | ---------------- | ------------------- |
  | 返回组织者发布的某个课程的详情，如参与人员，完成情况等 | GET /org/{org_id}/items/{item_id} | N/A              | {"item_detail": {}} |




- 发布课程或项目等

  | Description    | HTTP Mapping                 | HTTP RequestBody    | HTTP ResponseBody |
  | -------------- | ---------------------------- | ------------------- | ----------------- |
  | 组织者发布课程 | POST /org/{org_id}/items/add | {"item_detail": {}} | Empty             |




- 更新课程项目状态

  | Description                                            | HTTP Mapping                    | HTTP RequestBody | HTTP ResponseBody |
  | ------------------------------------------------------ | ------------------------------- | ---------------- | ----------------- |
  | 组织者更新课程或项目等，如对某位学习者学习成果进行认证 | POST /org/{org_id}/items/update | {"option": ""}   | Empty             |



> 以上“课程”包括课程、项目、竞赛、实习、活动等各种类型