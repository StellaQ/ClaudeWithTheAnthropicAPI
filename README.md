# Claude with Anthropic API

这是一个使用 Anthropic API 与 Claude AI 进行交互的 Jupyter Notebook 项目。

## 项目描述

本项目演示了如何：
- 安装和配置 Anthropic Python SDK
- 设置环境变量来保护 API 密钥
- 创建基本的聊天功能
- 与 Claude AI 模型进行对话

## 安装和设置

### 1. 克隆项目
```bash
git clone <your-repo-url>
cd ClaudeWithTheAnthropicAPI
```

### 2. 创建虚拟环境（推荐）
```bash
python3 -m venv venv
source venv/bin/activate  # macOS/Linux
# 或
venv\Scripts\activate     # Windows
```

### 3. 安装依赖
```bash
pip install anthropic python-dotenv
```

### 4. 设置环境变量
创建 `.env` 文件并添加你的 Anthropic API 密钥：
```
ANTHROPIC_API_KEY=your_api_key_here
```

**注意：** 请确保从 [Anthropic Console](https://console.anthropic.com/) 获取有效的 API 密钥。

## 使用方法

1. 启动 Jupyter Notebook：
   ```bash
   jupyter notebook
   ```

2. 打开 `001_requests.ipynb` 文件

3. 按顺序运行所有单元格：
   - 安装依赖包
   - 加载环境变量
   - 创建 API 客户端
   - 定义辅助函数
   - 开始与 Claude 对话

## 文件结构

- `001_requests.ipynb` - 主要的 Jupyter Notebook 文件
- `.env` - 环境变量文件（不会上传到 Git）
- `.gitignore` - Git 忽略文件配置
- `README.md` - 项目说明文档

## 功能特性

- **安全的 API 密钥管理**：使用环境变量保护敏感信息
- **简单易用的聊天接口**：封装了基本的消息发送和接收功能
- **模块化设计**：提供了添加用户消息、助手消息的辅助函数

## 注意事项

- 请确保不要将 `.env` 文件提交到版本控制系统
- API 调用会产生费用，请合理使用
- 建议在虚拟环境中运行项目

## 贡献

欢迎提交 Issue 和 Pull Request！

## 许可证

MIT License 