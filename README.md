视频关键帧与文本抓取工具 —— 基于 AI 自动从视频中抽取关键帧，并识别画面/字幕文本，将非结构化视频转化为可检索的结构化数据。

## 简介

**AI Video Keyframe & Text Extraction** 是一款基于 AI 的视频内容解析工具。它能够自动从长视频中抽取代表性关键帧，并识别画面中的文字、字幕等文本信息，将非结构化的视频内容转化为可检索、可分析的结构化数据，服务于视频内容理解、索引与检索等场景。

> An AI-powered tool that automatically extracts keyframes from videos and recognizes on-screen text and subtitles, converting unstructured video content into searchable, analyzable structured data.

## 功能特性

- **视频接入**：支持本地视频文件与在线视频源导入，兼容 MP4、MOV、AVI 等常见格式
- **关键帧抽取**：基于画面变化、场景切换等算法自动选取代表性关键帧，避免冗余帧
- **文本识别（OCR）**：对关键帧画面进行文字识别，提取标题、字幕、弹幕、PPT 文字等
- **语音/字幕文本提取**（可选）：结合 ASR 提取音频转文字，与画面文本合并
- **结构化输出**：输出「时间戳 + 关键帧图片 + 文本」的结构化结果，支持 JSON / CSV 导出
- **检索与索引**：基于提取的文本建立索引，支持按关键词定位视频片段

## 技术栈

> 按实际项目填写，以下为示例

- 语言：Python 3.9+
- 视频处理：OpenCV / FFmpeg
- 关键帧算法：场景检测（PySceneDetect 等）
- OCR：PaddleOCR / Tesseract
- ASR（可选）：Whisper
- 输出：JSON / CSV
- 依赖管理：pip / conda

## 安装

```bash
git clone https://github.com/你的用户名/ai-video-keyframe-text-extraction.git
cd ai-video-keyframe-text-extraction
pip install -r requirements.txt
