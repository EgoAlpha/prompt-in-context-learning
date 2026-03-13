# **第二十讲 Remotion skills**



**版本：**

python 3.12

langchain==1.2.1

deepagents-cli == 0.0.29

@remotion/cli == 4.0.434

## 1.检查node.js

```powershell
# 安装 Node.js（自动包含 npm）
winget install OpenJS.NodeJS.LTS
# 验证
node --version
npm --version
```

## 2.安装remotion

```bash
# 方法1：全局安装
npm install -g @remotion/cli

# 方法2：项目本地安装
npm install @remotion/cli

```

## 3.创建remotion项目

```bash
npx create-video@latest
```

## 4.查看deepagents 是否发现remotion skills

```powershell
deepagents skills list
```

## 5.启动deepagents

```bash
deepagents --model openai:deepseek-ai/DeepSeek-V3.2
```

## 6.手动预览

```bash
 npx remotion preview
```

## 7.手动渲染

```bash
npx remotion render
```

## 8.安装chrome依赖（linux系统可能需要此操作）

```bash
# 更新系统包
sudo apt-get update

# 安装 Chrome 所需的依赖库
sudo apt-get install -y \
  libnss3 \
  libnspr4 \
  libatk1.0-0 \
  libatk-bridge2.0-0 \
  libcups2 \
  libdrm2 \
  libxkbcommon0 \
  libxcomposite1 \
  libxdamage1 \
  libxfixes3 \
  libxrandr2 \
  libgbm1 \
  libasound2 \
  libpango-1.0-0 \
  libcairo2 \
  libatspi2.0-0
```

## 8.安装tailwind（可手动安装）

```bash
npm install @remotion/tailwind-v4
```

