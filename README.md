# MindCode 🧠⚡

[![Next.js](https://img.shields.io/badge/Next.js-14-black)](https://nextjs.org/)
[![ReactFlow](https://img.shields.io/badge/ReactFlow-可视化-ff0072)](https://reactflow.dev/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> **训练思维，编码未来。**  
> 一款面向 AI 时代的可视化计算思维训练平台。拆解逻辑、AI 导师陪练、分享思维路径。
- "在 AI 能写代码的时代，思维方式才是你唯一不可替代的核心竞争力。"

[在线演示](https://mindcode.top) · [开发文档](https://docs.mindcode.dev) · [问题反馈](https://github.com/BofanZhou/mindcode/issues)

![MindCode 截图](https://your-screenshot-url.png)

---

## ✨ 核心特性

### 🧩 可视化逻辑拆解
- **节点化画布**：拖拽式思维导图，支持开始、逻辑、处理、数据和结束节点
- **无限画布**：基于 ReactFlow 的工作空间，支持缩放、平移和小地图导航
- **智能布局**：自动排列复杂的逻辑树和算法结构

### 🤖 内联 AI 导师
- **几何化 AI 形象**：纯 CSS 构图的抽象机器人导师（苏格拉底式/伙伴式/分析师人格）
- **上下文引导**：AI 出现在选中节点旁边，而非侧边栏——真正的上下文对话
- **苏格拉底式提问**：AI 通过提问而非直接给答案，训练你的调试思维

### 🌊 社区与分享
- **瀑布流发现**：瀑布流布局展示社区思维导图
- **Fork 文化**：复刻他人的逻辑骨架用于自己的场景
- **社交功能**：点赞、评论、关注创作者；贡献值积分系统

### 📱 响应式设计优先
- **桌面端**：可折叠侧边栏（240px ↔ 72px）+ 画布 + 可折叠 AI 面板
- **移动端**：创新的可折叠最近地图头部 + 底部导出抽屉
- **自适应主题**：基于 CSS 变量的系统级深色/浅色模式

### 🎨 多模态导出
将思维成果导出为任意格式：
- **PNG/SVG**：高清截图便于分享（基于 html-to-image）
- **Markdown**：层级式文本大纲
- **代码**：生成 Python/JavaScript 伪代码
- **交互链接**：保留节点交互性的只读分享链接

---

## 🚀 快速开始

### 环境要求
- Node.js 18+
- Supabase 账号（数据库与认证）
- OpenAI API 密钥

### 安装

```bash
# 克隆仓库
git clone https://github.com/yourusername/mindcode.git
cd mindcode

# 安装依赖
npm install

# 配置环境变量
cp .env.example .env.local

# 运行开发服务器
npm run dev
```
---
## 🏗️ 项目结构

- **app/** — Next.js 14 App Router
  - **(main)/** — 主应用路由（带侧边栏布局）
    - **workbench/** — 画布编辑页
    - **community/** — 社区发现与分享
    - **profile/** — 用户主页与统计
    - **templates/** — 模板市场
  - **api/** — API 路由（AI、导出等）
  - **layout.tsx** — 根布局（含主题 Provider）

- **components/**
  - **ui/** — 设计系统（Button、Card、Input、Avatar）
  - **layout/** — 布局组件（Sidebar、AI Panel）
  - **canvas/** — ReactFlow 封装与自定义节点
  - **mobile/** — 移动端专用（CollapsibleHeader）
  - **export/** — 导出弹窗与抽屉
  - **community/** — 动态卡片、评论、筛选器

- **hooks/**
  - **useExport.ts** — PNG/SVG/Markdown/PDF 导出逻辑
  - **useAIChat.ts** — OpenAI 流式对话集成
  - **useLayout.ts** — 侧边栏折叠状态

- **lib/**
  - **utils.ts** — cn() 工具函数
  - **export/** — 各格式导出生成器
  - **constants.ts** — 示例流程、主题 Token

- **types/**
  - **index.ts** — TypeScript 类型定义

- **public/** — 静态资源
---

## 💻 技术栈

| 类别      | 技术                                                       | 说明                     |
| ------- | -------------------------------------------------------- | ---------------------- |
| **框架**  | [Next.js 14](https://nextjs.org/)                        | App Router、服务端组件       |
| **样式**  | [Tailwind CSS](https://tailwindcss.com/)                 | 原子化 CSS + CSS 变量主题     |
| **画布**  | [ReactFlow](https://reactflow.dev/)                      | 节点式图形编辑器               |
| **数据库** | [Supabase](https://supabase.com/)                        | PostgreSQL + 实时订阅 + 认证 |
| **AI**  | [OpenAI](https://openai.com/)                            | GPT-4o-mini 节点级陪练      |
| **动画**  | [Framer Motion](https://www.framer.com/motion/)          | 布局过渡与手势                |
| **导出**  | [html-to-image](https://github.com/bubkoo/html-to-image) | 画布截图生成                 |
| **图标**  | [Heroicons](https://heroicons.com/)                      | 线性图标库                  |

---

## 🎯 路线图
- [x] Phase 1: 设计系统与核心画布
- [x] Phase 2: 布局框架与响应式外壳
- [x] Phase 3: 社区功能与导出系统
- [ ] Phase 4: 实时协作（Yjs + WebRTC）
- [ ] Phase 5: 模板市场与 Pro 订阅
- [ ] Phase 6: MindCode DSL（领域专用语言）

---

## 🤝 参与贡献
我们欢迎各种形式的贡献！
- Fork 本仓库
- 创建特性分支 (git checkout -b feature/AmazingFeature)
- 提交改动 (git commit -m 'Add some AmazingFeature')
- 推送到分支 (git push origin feature/AmazingFeature)
- 创建 Pull Request
- 详情请参阅 CONTRIBUTING.md。

---

## 🙏 致谢
- ReactFlow 提供强大的节点编辑器
- Supabase 提供开源 Firebase 替代方案
- Tailwind Labs 提供原子化 CSS 框架
- Vercel 提供边缘部署与 Serverless 支持
- 独立开发者社区提供的宝贵反馈和功能建议
---
