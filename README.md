# MindCode 🧠⚡

[![Next.js](https://img.shields.io/badge/Next.js-14-black)](https://nextjs.org/)
[![ReactFlow](https://img.shields.io/badge/ReactFlow-可视化-ff0072)](https://reactflow.dev/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> **训练思维，编码未来。**  
> 一款面向 AI 时代的可视化计算思维训练平台。拆解逻辑、AI 导师陪练、分享思维路径。

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
