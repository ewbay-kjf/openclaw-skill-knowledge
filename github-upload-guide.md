# GitHub 上传指南

## 方法一：手动上传到 GitHub

### 步骤 1: 在 GitHub 创建新仓库
1. 访问 https://github.com/new
2. 创建新仓库，命名为 "openclaw-skill-knowledge"
3. 选择公开或私有仓库

### 步骤 2: 上传文件到 GitHub
你可以使用以下方式上传：

#### 网页上传
1. 在 GitHub 仓库页面点击 "Add file" → "Upload files"
2. 上传以下文件：
   - `技能知识库.md`
   - `skill-lookup.skill`
   - `skill-knowledge.tar.gz`
   - `README.md`

#### Git 命令行上传
如果你有 GitHub 账号和 SSH 密钥：
```bash
# 克隆你的仓库
git clone https://github.com/yourusername/openclaw-skill-knowledge.git

# 复制文件
cp /tmp/skill-knowledge/* /path/to/openclaw-skill-knowledge/

# 添加文件
cd /path/to/openclaw-skill-knowledge
git add .
git commit -m "Add OpenClaw skill knowledge base"
git push
```

## 方法二：使用 GitHub CLI

如果你安装了 GitHub CLI (`gh`)：

```bash
# 创建仓库
gh repo create openclaw-skill-knowledge --public --source=.

# 添加文件
git add .
git commit -m "Add OpenClaw skill knowledge base"
git push origin main
```

## 方法三：使用 GitHub Desktop

1. 下载 GitHub Desktop
2. 创建新仓库
3. 将文件拖入仓库
4. 提交并推送

## 获取文件

如果你直接从服务器获取文件：

```bash
# 复制文件到本地
scp root@your-server:/tmp/skill-knowledge/* .

# 或者下载压缩包
scp root@your-server:/root/.openclaw/workspace/skill-knowledge.tar.gz .
```

## 文件说明

### 1. `技能知识库.md`
完整的 OpenClaw 技能知识库，包含所有技能信息

### 2. `skill-lookup.skill`
打包好的技能文件，可以直接导入到 OpenClaw

### 3. `skill-knowledge.tar.gz`
包含所有内容的压缩包

### 4. `README.md`
使用说明文档

## GitHub 链接生成

上传后，你的 GitHub 仓库 URL 将是：
```
https://github.com/YOUR_USERNAME/openclaw-skill-knowledge
```

每个文件的直接链接：
```
https://github.com/YOUR_USERNAME/openclaw-skill-knowledge/blob/main/技能知识库.md
https://github.com/YOUR_USERNAME/openclaw-skill-knowledge/blob/main/skill-lookup.skill
https://github.com/YOUR_USERNAME/openclaw-skill-knowledge/blob/main/skill-knowledge.tar.gz
```

## 注意

如果你需要我帮你上传，你需要：
1. 提供 GitHub 个人访问令牌（PAT）
2. 或者提供 SSH 密钥
3. 或者授权我使用你的账户