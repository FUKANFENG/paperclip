# Paperclip 本地部署与 MiniMax 配置记录

这份文档记录一次本地 Paperclip 试用部署，不包含任何 API Key 或私密配置。

## 当前环境

- Paperclip：0.3.1
- 本地地址：http://127.0.0.1:3100
- 部署模式：local_trusted
- 数据库：嵌入式 PostgreSQL
- 模型：MiniMax-M3.1-Flash-Preview
- 适配器：Hermes Local
- 当前公司：OnePerson
- 当前智能体：MiniMax M3.1 试用员工

## 已完成验证

- MiniMax API 连通
- Paperclip 心跳运行
- 任务 ONE-1 执行完成
- 智能体评论写回任务
- 中文前端页面可用
- 服务重启后中文界面保持有效
- 数据库自动备份正常

## 中文界面方案

使用 Paperclip CN 的中文前端静态资源，同时保留当前 Paperclip 后端和数据库。这样可以避免直接替换社区 Fork 后端时出现数据库迁移版本冲突。

社区中文 Fork：

https://github.com/penclipai/paperclip-cn

## 安全说明

API Key 保存在本地加密 Secret 中，没有写入本仓库、README、Issue 或 Git 历史。

## 快速访问

启动后打开：

http://127.0.0.1:3100

如果浏览器显示旧页面，请执行强制刷新。