# 认知实验平台 (Cognitive Experiment Platform)

> 基于 Web 的认知行为实验平台，支持图片呈现和按键反应收集

## 项目简介

本项目是一个开源的认知行为实验平台，主要用于进行 MNIST 数字识别实验。平台支持：

- 用户注册/登录系统
- 练习模式（匿名用户）
- 正式实验（45轮 × 40试次）
- 断点续做（支持多天完成）
- 全屏实验环境
- 中断检测与处理
- 数据导出功能

## 技术栈

- **前端**: Vue 3 + Vite
- **后端**: FastAPI + SQLite
- **实验**: PsychoJS (改造后)
- **部署**: Docker + Nginx
- **域名**: cognitive-testing.cn

## 项目结构

```
cognitive-experiment-platform/
├── backend/           # FastAPI 后端
├── frontend/          # Vue 3 前端
├── nginx/             # Nginx 配置文件
├── psychojs/          # PsychoJS 实验文件
├── docs/              # 项目文档
│   └── 开发日志/       # 开发进度记录
├── data/              # 数据存储目录（不提交Git）
└── docker-compose.yml # Docker 部署配置
```

## 快速开始

### 本地开发

```bash
# 克隆仓库
git clone https://github.com/yourusername/cognitive-experiment-platform.git
cd cognitive-experiment-platform

# 启动服务
docker-compose up -d
```

### 访问地址

- 前端: http://localhost
- 后端 API: http://localhost/api

## 文档

- [实施计划](./docs/实施计划.md)
- [项目进度](./docs/项目进度.md)
- [开发日志](./docs/开发日志/)

## 开源协议

MIT License

## 联系方式

- 邮箱: dev@cognitive-testing.cn
- 域名: https://cognitive-testing.cn
