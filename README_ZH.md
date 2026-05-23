# KakutiResume - 现代简历编辑器

KakutiResume 是一个基于浏览器的、无需后端的简历编辑器。它结合了 **Notion 式的编辑体验** 和 **Typst 强大的排版能力**，为您提供实时预览、高性能 PDF 生成以及现代化的简历模板。

**🌐 在线使用: [https://resume.kakuti.site/](https://resume.kakuti.site/)**

---

[English](./README.md) | 简体中文 | [日本語](./README_JA.md)

---

## ✨ 核心特性

- **🚀 浏览器端 Typst 编译 (WASM)**: 所有的 PDF 生成逻辑都在您的浏览器中运行，无需服务器，保证了极高的隐私性和响应速度。
- **📝 Notion 风格块编辑器**: 支持文本、列表、标题等多种内容块，编辑体验流畅且直观。
- **📋 多模板支持**:
  - **日本标准履历书 (Rirekisho)** & **职务经历书 (Shokumukeirekisho)**。
  - **现代英文简历 (Western Style)**。
- **💾 本地持久化**: 您的数据实时保存于浏览器本地（LocalStorage/IndexedDB），无需担心数据丢失，且无需注册账号。
- **📂 Markdown 兼容**: 支持 Markdown 格式的导入与导出，方便数据迁移、版本控制和备份。
- **📱 响应式预览**: 实时查看 Typst 渲染出的 PDF/SVG 效果，所见即所得。

## 🛠️ 技术栈

- **框架**: [React](https://reactjs.org/) + [TypeScript](https://www.typescriptlang.org/)
- **构建工具**: [Vite](https://vitejs.dev/)
- **排版引擎**: [Typst](https://typst.app/) (通过 WASM 在浏览器内运行)
- **样式**: [Tailwind CSS](https://tailwindcss.com/)
- **状态管理**: React Hooks & Context API

## 🚀 快速开始

如果您想在本地运行本项目：

1. **安装依赖**:
   ```bash
   npm install
   ```

2. **启动开发服务器**:
   ```bash
   npm run dev
   ```

3. **访问**: 打开浏览器访问 `http://localhost:5173`。

## 📦 部署

本项目专为 Vercel 优化。您只需将代码推送至 GitHub 并关联 Vercel 项目，即可自动完成部署。根目录下的 `vercel.json` 已经配置好了构建指令。

---

> **架构说明**: 本项目已完成从后端编译到纯前端 WASM 编译的架构升级。原有的 `backend` 和 `typst-service` 目录已被移除，现在它是一个完全的静态单页应用 (SPA)。

## ⚠️ 免责声明

本工具仅负责解析 PDF 文件和生成排版好的 PDF 文件，不负责具体的简历内容。用户必须自行决定最终内容，并对简历文本的修改、纠错和真实性负全部责任。

完整免责声明请阅读：[免责声明 / Disclaimer](./DISCLAIMER.md)。

## 📄 开源协议

本项目采用 MIT 协议。
