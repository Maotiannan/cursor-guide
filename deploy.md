# 部署指南：将CURSOR小白行动指南发布到网络

本指南将帮助您将CURSOR小白行动指南网页部署到GitHub Pages，这样您就可以在任何设备（包括手机）上访问它。

## 方法一：使用GitHub Pages（免费，推荐）

### 步骤1：创建GitHub账号

如果您还没有GitHub账号，请前往 [GitHub官网](https://github.com/) 注册一个账号。

### 步骤2：创建新仓库

1. 登录GitHub后，点击右上角的"+"图标，选择"New repository"
2. 仓库名称填写：`cursor-guide`（或您喜欢的任何名称）
3. 保持仓库为"Public"（公开）
4. 点击"Create repository"创建仓库

### 步骤3：上传文件

有两种方式上传文件：

#### 方式A：使用GitHub网页界面（简单）

1. 在新创建的仓库页面，点击"Add file"→"Upload files"
2. 将您的`index.html`和`styles.css`文件拖拽到上传区域
3. 在下方的"Commit changes"区域添加描述（如"Initial upload"）
4. 点击"Commit changes"按钮提交文件

#### 方式B：使用Git命令行（高级）

如果您熟悉Git，可以使用以下命令：

```bash
# 克隆仓库
git clone https://github.com/您的用户名/cursor-guide.git
cd cursor-guide

# 复制文件到仓库文件夹
# 然后添加并提交文件
git add .
git commit -m "Initial commit"
git push origin main
```

### 步骤4：启用GitHub Pages

1. 在仓库页面，点击"Settings"
2. 在左侧菜单中，点击"Pages"
3. 在"Source"部分，选择"main"分支，文件夹选择"/(root)"
4. 点击"Save"按钮
5. 等待几分钟，GitHub会显示您的网站URL（通常是`https://您的用户名.github.io/cursor-guide/`）

### 步骤5：访问您的网站

使用GitHub Pages提供的URL，您现在可以在任何设备上访问您的CURSOR小白行动指南，包括手机、平板和电脑。

## 方法二：使用Netlify Drop（免费，超简单）

如果您想要更简单的方法，可以使用Netlify Drop：

1. 访问 [Netlify Drop](https://app.netlify.com/drop)
2. 将您的`index.html`和`styles.css`文件拖拽到网页中的上传区域
3. Netlify会自动部署您的网站并提供一个URL
4. 您可以点击"Site settings"→"Change site name"来自定义URL

## 方法三：使用Vercel（免费，功能丰富）

Vercel也提供免费托管：

1. 访问 [Vercel](https://vercel.com/) 并使用GitHub账号登录
2. 点击"New Project"
3. 导入您的GitHub仓库（如果您已经按照方法一上传了文件）
4. 点击"Deploy"
5. Vercel会自动部署您的网站并提供一个URL

## 更新网站内容

无论您选择哪种部署方法，当您需要更新网站内容时：

1. 修改本地的`index.html`或`styles.css`文件
2. 按照您选择的部署方法重新上传或提交更改
3. 网站将自动更新

## 注意事项

- GitHub Pages可能需要几分钟时间来部署您的更改
- 确保您的文件名大小写正确，特别是`index.html`必须全部小写
- 如果您添加了图片或其他资源，确保在HTML中使用相对路径引用它们 