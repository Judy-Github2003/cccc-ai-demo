# 中交 AI Demo

本仓库用于两人协作开发中交 AI Demo。目前仅建立协作骨架，业务功能、接口实现和运行环境尚未实现，暂不能按此仓库直接启动服务。

## 业务范围

- 立项材料审查：提交材料、执行审查并查看结果。
- 立项书起草：根据输入材料生成可审阅的草稿。
- Excel 拆表：上传工作簿并生成拆分结果。

计划统一后端服务与任务处理机制，WorkBuddy 作为调用入口；具体接入方式待实现。

## 技术栈与分工

技术栈已确定为 Java + Spring、Next.js + React、MongoDB、Apifox、Git 和 Docker。具体版本与依赖配置待补齐。

- A：后端公共接口、任务机制、材料审查及模型接入。
- B：前端开发与联调，并协助 Excel 拆表。
- 共同：立项书起草、部署与验收。

通过共同需求、Apifox 接口契约和 Git 代码协作；各自的个人 GPT 对话不作为项目唯一依据。

## 目录约定

```text
backend/    后端服务
frontend/   前端应用
deploy/     部署配置
apifox/     接口契约与可共享导出文件
config/     配置模板
templates/  可公开提交的业务模板
docs/       需求与开发说明
tests/      测试代码与脱敏测试样例
```

上述目录用于约定代码归属，不代表对应能力已经实现。原始客户素材、生成输出、密钥及含敏感信息的配置不得提交。

## 获取与协作

```bash
git clone https://github.com/Judy-Github2003/cccc-ai-demo.git
cd cccc-ai-demo
```

这是公开仓库，可直接 clone；开发约定见 [开发协作说明](docs/development.md)。

下一步先确认接口契约，再补齐固定版本、依赖锁文件和 Docker 运行配置，随后实现与验证业务流程。
