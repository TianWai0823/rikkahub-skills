---
name: openvl
description: 让无视觉能力的 AI 模型看懂图片。支持本地图片、URL、剪贴板截图、base64 数据、stdin 管道。用户提问会传给视觉模型直接回答。也支持 MCP 服务器供 Cherry Studio 等工具调用。
---

# Open Visual Language (OpenVL)

## 概述
让不具备视觉能力的 AI 模型能够看懂图片、处理图像输入。适用于 Claude Opus/Sonnet（Anthropic API 或 API 代理）、GPT-4 Vision 及其他纯文本模型。

## 工作流程
1. 检测用户请求中的图片来源（路径、URL、base64、剪贴板）
2. 根据具体场景调用视觉模型或工具
3. 将视觉模型的理解返回给用户

## 触发条件
- 用户提供了图片路径、URL 或 data URI
- 用户粘贴了图片到剪贴板
- 用户问图片内容、文字、场景、出处等
- 需要 OCR 提取图中的文字
- 需要分析图表、截图、UI 界面等
