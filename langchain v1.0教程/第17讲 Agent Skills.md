# **第十七讲 Agent工程概念  ——  Agent skills**



**版本：**

ubuntu 22.04

python 3.12

langchain==1.2.0

deepagents == 0.3.5

deepagents-cli 版本0.1.3

## 1.安装wsl

按照视频步骤检查系统配置之后才可运行

```bash
wsl --install
```

## 2.安装python 3.12

在linux子系统中运行

```bash
#添加Python官方PPA

sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update

 #安装Python 3.12

sudo apt install -y python3.12 python3.12-venv python3.12-dev
```

## 3.从github下载deepagent库



```bash
git clone https://github.com/langchain-ai/deepagents deepagents-demo
cd deepagents-demo
```

下载完成后，根据视频指引，修改deepagents-demo\libs\deepagents-cli\pyproject.toml中的字段版本配置

## 4.配置虚拟环境

```bash
#创建3.12虚拟环境

python3.12 -m venv langchain-skills

#激活虚拟环境

source langchain-skills/bin/activate

#验证Python版本

python --version  

#确保大于等于 python 3.12版本
```

## 5.安装库（确保处于linux中新建的虚拟环境）

```bash
#安装库：

pip install -e libs/deepagents

pip install -e libs/deepagents-cli

pip install langchain-openai
```

## 6.观察安装版本

```bash
#观察版本：
#deepagents 0.3.5
#deepagents-cli 0.1.2
pip show deepagents

pip show deepagents-cli
```

## 7.配置环境变量

```bash
#填入自己的环境变量
export LANGSMITH_TRACING=true
export LANGSMITH_API_KEY=lsv2_...
export OPENAI_BASE_URL=https://...
export OPENAI_API_KEY=sk-...
export TAVILY_API_KEY=tvly-...
```

## 8.下载langchain官方skill示例（确保路径处于deepagents-demo）

```bash
#下载skills：

mkdir -p .deepagents

cp -r libs/deepagents-cli/examples/skills .deepagents/skills/
```

## 9.检查skill是否可发现

```bash
deepagents skills list
```

## 10.启动deepagents

```bash
deepagents --model gpt-5
```
