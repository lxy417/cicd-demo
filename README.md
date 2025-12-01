# React + Vite TodoList Demo

一个使用 React + Vite 构建的现代化 TodoList 应用，通过 GitHub Actions 自动构建并部署到 GitHub Pages。

## 功能特性

- ✅ 添加待办事项
- ✅ 标记完成/未完成
- ✅ 删除待办事项
- ✅ 统计信息显示
- ✅ 响应式设计
- ✅ 现代化 UI 界面

## 技术栈

- React 18
- Vite 5
- GitHub Actions (CI/CD)
- GitHub Pages (部署)

## 本地开发

### 安装依赖

```bash
npm install
```

### 启动开发服务器

```bash
npm run dev
```

### 构建生产版本

```bash
npm run build
```

### 预览生产构建

```bash
npm run preview
```

## GitHub Pages 部署

### 设置步骤

1. **启用 GitHub Pages**
   - 进入仓库的 Settings
   - 找到 Pages 选项
   - 在 Source 中选择 "GitHub Actions"

2. **推送代码到 GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin <your-repo-url>
   git push -u origin main
   ```

3. **自动部署**
   - 当代码推送到 `main` 分支时，GitHub Actions 会自动构建并部署
   - 部署完成后，可以在仓库的 Settings > Pages 中查看部署地址

### 重要提示

⚠️ **注意**: 在 `vite.config.js` 中，`base` 路径需要与你的仓库名称匹配。如果仓库名称不是 `react-vite-todolist`，请修改 `vite.config.js` 中的 `base` 配置。

例如，如果仓库名称是 `my-todolist`，则应该设置为：
```js
base: '/my-todolist/',
```

## 项目结构

```
.
├── src/
│   ├── App.jsx          # 主应用组件
│   ├── App.css          # 应用样式
│   ├── main.jsx         # 入口文件
│   └── index.css        # 全局样式
├── .github/
│   └── workflows/
│       └── deploy.yml   # GitHub Actions 工作流
├── index.html           # HTML 模板
├── vite.config.js       # Vite 配置
└── package.json         # 项目依赖
```

## License

MIT

