# 杰西亚费用监控系统 - 前端

静态HTML前端，部署到 Netlify 免费托管。

## 部署到 Netlify

### 方法一：从GitHub部署（推荐）

1. 将此仓库推送到 GitHub
2. 登录 [Netlify.com](https://netlify.com)（用GitHub登录）
3. 点击 "Add new site" → "Import an existing project"
4. 选择 GitHub，授权后选择此仓库
5. 配置：
   - **Build command**:（留空）
   - **Publish directory**: `.`（当前目录）
6. 点击 "Deploy"
7. 部署完成后，复制生成的URL（如 `https://jsy-expense.netlify.app`）
8. **重要**：修改 `index.html` 第8行的 `API_BASE`，把 `jsy-expense-api.onrender.com` 改成你实际的Render后端URL

### 方法二：拖拽部署（最快）

1. 登录 Netlify
2. 直接把 `frontend` 文件夹拖拽到 Netlify 的部署页面
3. 部署完成！
4. **重要**：修改 `index.html` 中的后端API地址为你实际的Render URL

## 本地测试

直接用浏览器打开 `index.html` 即可（需配合本地后端 `http://localhost:3000` 使用）。

## 注意事项

- 前端是纯静态文件，无需构建
- 后端API地址配置在 `index.html` 第8行的 `API_BASE` 变量
- 部署后记得更新 `API_BASE` 为你的 Render 后端 URL
