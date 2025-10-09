# 🚀 Nimble - 轻快的临时文件与文本分享系统

> **Nimble**：瞬间共享，即刻送达。一个简洁、安全、开源的临时文件与文本分享工具。

---

## 📦 项目组成

Nimble 采用模块化设计，各组件独立开发、独立部署，便于维护与扩展：

| 仓库 | 功能 | 技术栈 |
|------|------|--------|
| [`nimble-frontend`](https://github.com/QingShanFrost/nimble-frontend) | 网页端界面 | Nuxt.js |
| [`nimble-backend`](https://github.com/QingShanFrost/nimble-backend) | 核心 API 服务 | Flask + PostgreSQL + Redis |
| [`nimble-client`](https://github.com/QingShanFrost/nimble-client) | 桌面客户端（Tauri） | Rust + Vue/React |
| [`nimble-db`](https://github.com/QingShanFrost/nimble-db) | 数据库 Schema 与迁移 | SQL |
| [`nimble-docs`](https://github.com/QingShanFrost/nimble-docs) | 本仓库：文档中心 | Markdown |

---

## 🚦 当前状态

🚧 **项目正在开发中**，核心功能尚未完成。

- ✅ 项目架构设计完成
- ✅ 仓库已创建
- 🔜 即将实现：
  - 文件/文本上传
  - 自动生成短链
  - 自动过期机制
  - GitHub/Gitee 登录支持

---

## 🛠️ 如何参与开发？

### 1. 克隆所有仓库（可选）

```bash
mkdir nimble && cd nimble
git clone https://github.com/QingShanFrost/nimble-frontend.git
git clone https://github.com/QingShanFrost/nimble-backend.git
git clone https://github.com/QingShanFrost/nimble-client.git
git clone https://github.com/QingShanFrost/nimble-db.git

2. 本地开发建议
后端：启动 nimble-backend，确保数据库连接正常
前端：在 nimble-frontend 中配置 API_URL=http://localhost:5000
客户端：使用 Tauri 开发模式运行 nimble-client
详细开发指南见各仓库的 README.md。

📥 部署计划（未来）
支持多种部署方式：

本地一键启动：docker-compose up
生产环境：Nginx + Gunicorn + PostgreSQL
自定义实例：支持反向代理、HTTPS、自定义域名
🤝 贡献
欢迎贡献！你可以：

提交 Issue（功能建议、Bug 报告）
提 PR（修复、文档、新功能）
设计 Logo 或 UI
请先阅读 CONTRIBUTING.md（即将创建）。

📄 许可证
本项目采用 Apache License 2.0 开源。这意味着你可以在遵循该许可证的条件下自由地使用、修改和分发本软件。更多详情，请参阅 LICENSE 文件。

🌟 Nimble —— 因为分享，应该轻而易举。

text
编辑

---

## ✅ 下一步操作清单

1. **创建 LICENSE 文件**
   - 在每个仓库根目录下创建 `LICENSE` 文件
   - 内容为 Apache License 2.0 的全文
   - 获取地址：https://www.apache.org/licenses/LICENSE-2.0.txt
   - 或使用 GitHub 创建仓库时自带的模板

2. **创建 `nimble-docs/assets/` 目录**
   ```bash
   mkdir -p nimble-docs/assets
未来可存放架构图、Logo 等资源
将上述 README.md 内容粘贴到 nimble-docs 仓库
在其他四个仓库的 README.md 中添加链接回 nimble-docs
🎁 小贴士
你可以使用 Excalidraw 绘制手绘风格的架构图，导出为 architecture.png 放入 assets/
建议在 nimble-backend 和 nimble-frontend 的 README.md 中也引用 Apache 2.0 许可证
