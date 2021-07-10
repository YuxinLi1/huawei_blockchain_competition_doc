# 代码架构

目录：

```shell
code
├── chaincode.go								# 链代码
└── server										# 后端
	├── api
	│   ├── common								# 公用接口
	│   ├── contract							# 合约调用接口
	│   ├── learner								# 学习者接口
	│   ├── organization						# 组织机构接口
	│   └── registration						# 注册登录接口
	├── config
	├── db
	├── locales
	├── main.go
	└── schema
```



详细内容：

```shell
code
├── chaincode.go								# 链代码
└── server										# 后端
	├── api
	│   ├── common								# 公用接口
	│   │   ├── certs.query.handler.go				# 证书查询验证
	│   │   └── index.handler.go					# 首页
	│   ├── contract							# 合约调用接口
	│   │   ├── config								# 华为链配置文件
	│   │   ├── config.go							# 配置信息
	│   │   ├── contract_test.go					# 合约接口测试
	│   │   ├── query.go							# 查询
	│   │   ├── send.go								# 上链
	│   │   └── utils.go
	│   ├── learner								# 学习者接口
	│   │   ├── learner.certs.handler.go			# 学习者证书
	│   │   ├── learner.items.detail.handler.go		# 参与的课程的详情
	│   │   ├── learner.items.handler.go			# 推荐课程
	│   │   ├── learner.items.mine.handler.go		# 参与课程
	│   │   └── learner.items.update.handler.go		# 课程状态更新
	│   ├── organization						# 组织机构接口
	│   │   ├── org.items.add.handler.go			# 发布课程、项目、实习、活动、竞赛
	│   │   ├── org.items.detail.handler.go			# 单个item的详情
	│   │   ├── org.items.handler.go				# 发布的所有item
	│   │   └── org.items.update.handler.go			# 更新信息
	│   └── registration						# 注册登录接口
	│       ├── login.handler.go					# 登录
	│       ├── logout.handler.go					# 登出
	│       └── register.handler.go					# 注册
	├── config
	│   ├── config.ENV.json
	│   └── config.go
	├── db
	├── locales
	│   ├── en.json
	│   └── fr.json
	├── main.go
	└── schema
		└── schema.go

```

