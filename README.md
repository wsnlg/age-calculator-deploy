# 年龄计算器

> 输入出生日期（支持阳历/农历），精确计算你活过的每一秒

## ✨ 功能特性

- 📅 **阳历/农历切换** — 支持双历法输入，自动对照显示
- ⏱️ **精准计算** — 实时秒级更新，精确到年月日时分秒
- 🎂 **生日倒计时** — 阳历 + 农历双生日倒计时
- ✨ **星座生肖** — 自动识别西方星座和中国生肖
- 📊 **生命统计** — 心跳、呼吸、眨眼、睡眠等趣味数据
- 📈 **生命进度** — 可视化进度条，自定义预期寿命
- 🌙 **深色主题** — 支持深色/浅色主题切换
- 📱 **响应式** — 适配手机和桌面端

## 🚀 部署到 GitHub Pages

### 方式一：网页操作（推荐新手）

#### 第 1 步：创建 GitHub 仓库

1. 打开 [github.com](https://github.com)，登录账号（没有就注册一个）
2. 点击右上角 **+** → **New repository**
3. 仓库名称填：`age-calculator`
4. **重要**：选择 **Private**（私有仓库，保护源码）
5. **不要**勾选 "Add a README file"
6. 点击 **Create repository**

#### 第 2 步：上传文件

1. 进入刚创建的仓库页面
2. 点击 **Add file** → **Upload files**
3. 把以下 4 个文件拖拽上传：
   - `index.html`（主页面，混淆后的版本）
   - `.nojekyll`
   - `.gitignore`
   - `README.md`
4. 填写 Commit message（如 "初始部署"）
5. 点击 **Commit changes**

#### 第 3 步：开启 GitHub Pages

1. 进入仓库页面
2. 点击 **Settings**（设置）
3. 左侧菜单找到 **Pages**
4. 在 "Build and deployment" 下：
   - **Source** 选择 **Deploy from a branch**
   - **Branch** 选择 `main`，文件夹选 `/ (root)`
5. 点击 **Save**
6. 等待 1-2 分钟，页面顶部会显示你的网站链接：
   `https://你的用户名.github.io/age-calculator/`

---

### 方式二：命令行操作（有 Git 经验）

```bash
# 1. 创建仓库后，在本地执行：
git clone https://github.com/你的用户名/age-calculator.git
cd age-calculator

# 2. 把 index.html、.nojekyll、.gitignore、README.md 复制进来
# （从 age-calculator-deploy 目录复制）

# 3. 提交并推送
git add .
git commit -m "初始部署"
git branch -M main
git push -u origin main

# 4. 然后在 GitHub 网页上按上面第 3 步开启 Pages
```

---

### 更新页面

修改 `index.html` 后，重新上传或 push 即可。GitHub Pages 会自动重新部署（通常 1-3 分钟生效）。

## 🔒 源码保护说明

| 措施 | 说明 |
|------|------|
| **私有仓库** | 别人无法访问你的 GitHub 仓库，看不到源码 |
| **代码混淆** | `index.html` 已混淆压缩，变量名被替换，难以阅读 |
| **禁用右键** | 页面禁止右键"查看源代码" |
| **禁用快捷键** | 禁止 F12、Ctrl+Shift+I/J/C、Ctrl+U |
| **禁用选中** | 禁止选中页面文字 |

> ⚠️ **重要提醒**：纯前端代码理论上无法完全防止被查看（浏览器必须下载代码才能渲染），以上措施只能大幅增加难度。**私有仓库是最关键的保护**。

## 📁 文件说明

```
age-calculator/
├── index.html    ← 部署用的页面（已混淆，24.9KB）
├── .nojekyll     ← 告诉 GitHub Pages 不要用 Jekyll 处理
├── .gitignore    ← Git 忽略规则
└── README.md     ← 本文件
```
