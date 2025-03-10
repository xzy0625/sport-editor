# 运动步数修改工具

[![sport-editor-task](https://github.com/Devifish/sport-editor/actions/workflows/sport-editor-task.yml/badge.svg)](https://github.com/Devifish/sport-editor/actions/workflows/sport-editor-task.yml)
[![star](https://img.shields.io/github/stars/Devifish/sport-editor.svg?logo=github)](https://github.com/Devifish/sport-editor)
[![license](https://img.shields.io/github/license/Devifish/sport-editor)](https://github.com/Devifish/sport-editor)

> 通过华米运动的 API 提交运动步数 <br/>
> 可实现同步运动步数至热门平台，如微信、支付宝等 

## 实现功能 

- [x] 每日自动更新步数 
- [x] 指定随机运动步数范围
- [x] Github Action 运行

## 配置参数

| 环境变量                 | 说明                | 值                  |
| ------------------------ | ------------------- | ------------------- |
| XIAOMI_AMAZFIT_USERNAME  | 用户名              | 159000000           |
| XIAOMI_AMAZFIT_PASSWORD  | 密码                | xxxxxx              |
| XIAOMI_AMAZFIT_USER_ID   | 用户 ID (可选)      | 123456              |
| XIAOMI_AMAZFIT_APP_TOKEN | APP Token (可选)    | xxxxxxxx            |
| STED_SIZE_RANGE          | 运动步数范围 (可选) | 5000-15000 (默认值) |

- 推荐使用 Node.js 12 及以上的运行/构建当前项目
- 运动步数范围使用 - 分隔上下限
- 可选账号/密码、UserID/AppToken 两种方式运行

## Github Actions 部署

- fork 本项目
- 将环境变量参数填到 Setting -> Secrets (如果使用 Token+ID 方式可不填用户名及密码)
- 开启 actions (默认`actions`处于禁止状态)
- 执行 sport-editor-task workflow

## 命令行运行

```
git clone https://github.com/Devifish/sport-editor.git
cd sport-editor
npm install
npm run start
```
