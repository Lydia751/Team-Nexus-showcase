# Team Nexus 项目说明

Team Nexus 是一个面向团队协作的实时工作平台，主要覆盖工作区管理、看板任务管理、团队聊天、通知提醒和共享文件等场景。

本仓库用于项目展示与课程/学习成果归档，重点呈现系统功能、界面截图、架构设计和核心业务流程。

---

## 功能概览

- 工作区创建与管理
- Kanban 看板式任务协作
- 任务详情编辑、分配与状态跟踪
- 团队实时聊天
- 通知中心与协作事件提醒
- 工作区文件共享与上传
- Socket.IO 实时同步
- 基于 JWT 的用户认证

---

## 技术栈

### 前端

- React
- Vite
- Tailwind CSS
- Socket.IO Client
- Axios

### 后端

- Node.js
- Express.js
- MongoDB
- Mongoose
- Socket.IO
- multer
- JWT

---

## 仓库结构

```text
Team-Nexus-showcase-main/
+-- architecture/
|   +-- README.md
|   +-- system-architecture-diagram.png
|   +-- database-er-diagram.png
|   +-- task-workflow-diagram.png
+-- screenshots/
|   +-- README.md
|   +-- workspace-dashboard.png
|   +-- kanban-board.png
|   +-- task-list.png
|   +-- task-detail-modal.png
|   +-- shared-files.png
|   +-- notifications-page.png
|   +-- chat-page.png
+-- README.md
```

---

## 各部分说明

### architecture

`architecture` 目录用于说明 Team Nexus 的技术架构、数据库关系和任务协作流程。该部分适合用于答辩、项目文档、系统设计说明和开发交接。

包含内容：

- 系统架构图
- MongoDB 核心 ER 关系图
- 工作区与任务管理流程图
- 主要 API、Socket.IO 事件和模块说明

详细说明见：[architecture/README.md](./architecture/README.md)

### screenshots

`screenshots` 目录用于展示 Team Nexus 的主要界面和功能效果。该部分适合用于项目展示、作品集、演示材料和 README 功能预览。

包含内容：

- 工作区首页
- Kanban 任务看板
- 个人任务列表
- 任务详情弹窗
- 共享文件页面
- 通知中心
- 团队聊天页面

详细说明见：[screenshots/README.md](./screenshots/README.md)

---

## 核心业务流程

1. 用户登录后获取 JWT，并进入个人工作区列表。
2. 用户可以创建工作区，系统自动生成对应任务看板。
3. 团队成员在看板中创建任务、分配负责人、设置时间和更新完成状态。
4. 任务、通知和聊天消息通过 REST API 与 Socket.IO 进行同步。
5. 工作区成员可以查看共享文件、通知和团队沟通记录。

---

## 使用说明

本仓库主要用于展示，不包含完整运行环境、依赖目录和敏感配置文件。

如需运行完整项目，需要准备前端、后端、数据库和环境变量配置，包括：

- MongoDB 连接地址
- JWT 密钥
- 文件上传目录
- 前后端 API 地址
- Socket.IO 服务地址

---

## 备注

本项目仅用于学习、展示和教育目的。

仓库中的文档、截图、架构图和项目说明未经作者书面许可，不得复制、修改、二次分发或用于商业用途。
