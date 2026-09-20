# Agent Workflow Automation

一个用于自动化AI Agent工作流的开源工具集，支持任务调度、浏览器自动化、内容发布和数据处理。

## 特性

- 自动化任务调度（定时/触发器）
- 浏览器自动化脚本库
- 多平台内容发布（公众号、小红书、抖音）
- 数据处理和转换工具
- Agent间协作流程编排

## 使用场景

- AI Agent工作流自动化
- 社交媒体内容批量发布
- 网页数据采集和处理
- 任务调度和提醒

## 安装

```bash
pip install agent-workflow-automation
```

## 快速开始

```python
from agent_workflow import Workflow, Task

# 创建自动化流程
wf = Workflow("content-publish")
wf.add_task(Task("fetch-content", source="wechat"))
wf.add_task(Task("generate-post", llm="true"))
wf.add_task(Task("publish", platform=["wechat", "xhs"]))
wf.run()
```

## 许可证

MIT License
