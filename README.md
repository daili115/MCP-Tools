# MCP Tools

A curated collection of 100 Model Context Protocol (MCP) servers/tools with standardized install JSONs, complete metadata, and CI validation.

## Structure
- `/tools/index.json` — full metadata for all collected tools (name, version, description, author, compatibility, category)
- `/configs/tools-install.json` — standardized install configurations for each tool
- `.github/workflows/validate-configs.yml` — CI to validate JSON format and required fields
- `LICENSE` — MIT License
- `.gitignore` — standard ignores

## Categories
- Aggregators, File Systems, Browser Automation, Databases, Cloud Storage, Communication, Version Control, Monitoring, Search & Web, Productivity, Social Media, Finance, Dev Tools, Data Visualization, Identity, Security, IoT, Art & Media, E‑Commerce, Data Platforms, Robotics

## Usage
- Pick a tool from `/tools/index.json`
- Check its install commands in `/configs/tools-install.json`
- Add the server to your MCP client configuration (e.g., Claude Desktop `claude_desktop_config.json` under `"mcpServers"`)

## Notes
- Compatibility: MCP v1 unless otherwise stated. Most entries work with Claude Desktop, Zed, Cursor, Cody, etc.
- Versions are set to `latest` unless upstream provides explicit releases.
- Sources: Official MCP servers and curated community lists [modelcontextprotocol/servers], [awesome-mcp-servers] and related.

## Contribution
PRs welcome to update metadata, add servers, or improve install commands.

---

## 工具目录（参考 Awesome MCP Servers 风格）

以下为当前已收录的 MCP 工具清单，按类别分组展示，并附简要说明。完整来源与更多细节（版本、兼容性、作者等）请参见 `tools/index.json`。

### 官方与基础工具
- `@modelcontextprotocol/server-filesystem` — 本地受控文件系统访问（白名单路径）
- `@modelcontextprotocol/server-memory` — 持久化记忆与知识图谱
- `@modelcontextprotocol/server-git` — Git 仓库检查与操作
- `@modelcontextprotocol/server-fetch` — 抓取网页并转换为LLM可消费内容
- `mcp-server-git` — Git 服务器工具的 Python 实现
- `mcp-server-time` — 时间与时区转换工具
- `mcp-server-sequential-thinking` — 反思与序列化问题求解流程

### 代码与版本管理
- `@modelcontextprotocol/server-github` — GitHub 仓库与API集成
- `@modelcontextprotocol/server-gitlab` — GitLab API 集成
- `bitbucket-mcp` — Bitbucket API 集成
- `linear-mcp` — Linear 任务与项目集成

### 监控与可观测性
- `@modelcontextprotocol/server-sentry` — Sentry 问题检索与分析
- `alertmanager-mcp` — Prometheus Alertmanager 集成

### 通讯与协作
- `@modelcontextprotocol/server-slack` — Slack 频道与消息
- `gmail-mcp` — Gmail 邮件检索与发送

### 地图与位置服务
- `@modelcontextprotocol/server-google-maps` — 地理位置、路线、地点详情

### 搜索与网页
- `@modelcontextprotocol/server-brave-search` — Brave 搜索
- `autogen-docs-mcp` — 搜索并检索 Microsoft AutoGen 文档
- `bing-webmaster-mcp` — Bing Webmaster SEO 洞察
- `google-news-mcp` — Google News 搜索
- `kagi-search-mcp` — Kagi Search 集成
- `exa-search-mcp` — Exa AI 搜索集成
- `serpapi-mcp` — SERP API（Scrapeless）
- `@modelcontextprotocol/server-fetch` — 网页抓取整理（再次列出以强调）

### 浏览器自动化
- `@modelcontextprotocol/server-puppeteer` — 基于 Puppeteer 的浏览器自动化与抓取
- `browser-mcp` — 本地浏览器动作自动化
- `browser-mcp-puppeteer` — Puppeteer 自动化（含可访问性树）

### 云与系统自动化
- `aws-ec2-pricing-mcp` — 获取当前 EC2 价格信息
- `docker-mcp` — 管理 Docker 容器与镜像
- `kubernetes-mkp` — 访问与操作 Kubernetes 集群（StacklokLabs/mkp）
- `helm-mcp` — 管理 Helm Charts
- `terraform-mcp` — 基础设施即代码（Terraform）
- `android-adb-mcp` — 通过 ADB 控制 Android 设备

### 数据库与向量检索
- `airtable-mcp` — 读写 Airtable（含表结构检查）
- `bigquery-mcp` — Google BigQuery 查询访问
- `pinecone-mcp` — Pinecone 向量数据库集成
- `qdrant-mcp` — Qdrant 向量检索
- `milvus-mcp` — Milvus 向量数据库集成
- `weaviate-mcp` — Weaviate 向量数据库集成
- `mongodb-mcp` — MongoDB 查询与分析
- `postgres-mcp` — PostgreSQL 访问（含Schema检查）
- `cockroachdb-mcp` — CockroachDB 管理与查询

### 云存储
- `box-mcp` — Box 内容访问与管理
- `google-drive-mcp` — Google Drive 文件访问与搜索

### 生产力与日程
- `anki-connect-mcp` — 通过 AnkiConnect 操作 Anki
- `apisix-mcp` — 管理 Apache APISIX（Admin API）
- `apple-notes-mcp` — 访问本地 Apple 备忘录（macOS）
- `apple-shortcuts-mcp` — 集成 Apple 快捷指令
- `basecamp-mcp` — 管理 Basecamp 项目、待办与文档
- `calcom-mcp` — 通过 API 管理 Cal.com 排程
- `canvas-lms-mcp` — Canvas LMS 教学数据访问
- `caldav-mcp` — 通过 CalDAV 进行日历操作
- `jira-mcp` — 检索与管理 Jira 事项
- `notion-mcp` — Notion API 集成
- `todoist-mcp` — Todoist 自然语言任务管理
- `trello-mcp` — 管理 Trello 看板与卡片
- `asana-mcp` — Asana 项目与任务集成
- `monday-mcp` — Monday.com 工作区集成
- `clickup-mcp` — ClickUp 任务与文档集成
- `google-sheets-mcp` — 访问与编辑 Google Sheets
- `google-calendar-mcp` — 管理 Google Calendar 事件

### 社媒与内容平台
- `bluesky-mcp` — 检索与搜索 Bluesky 动态/帖子
- `reddit-mcp` — Reddit API 搜索与内容检索
- `x-twitter-mcp` — X/Twitter API 集成

### 开发者工具
- `clj-kondo-mcp` — Clojure Linter 集成
- `clojars-mcp` — 获取最新 Clojure 依赖详情
- `clojure-repl-mcp` — 通过 REPL 提供 Clojure 开发工具

### 安全与身份
- `binary-ninja-mcp` — Binary Ninja 插件与 MCP 桥接
- `bloodhound-mcp` — 通过 BloodHound 分析 AD 攻击路径
- `chaitin-ip-intel-mcp` — 基于长亭 API 的 IP 情报检索

### 可视化与实用小工具
- `chart-mcp` — 以类型安全配置生成图表
- `calculator-mcp` — 精确数值计算

### 金融与区块链
- `algorand-mcp` — 访问 Algorand 区块链工具与资源
- `coincap-mcp` — 通过 CoinCap 获取加密货币市场数据

---

说明：
- 为保持 README 清晰可读，以上为当前主要工具的“Awesome 列表”式展示；更多条目与字段细节请直接查看 `tools/index.json`（包含完整数组与元数据）。
- 如果需要完全按照 `awesome-mcp-servers` 的细粒度链接形式（逐条指向各上游仓库），可以在后续 PR 中补充链接信息或通过脚本从索引自动生成。
