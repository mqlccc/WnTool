# WnTool
# Linux服务器批量运维管理工具

一个基于Python和PyQt6开发的Linux服务器批量运维管理工具，提供可视化界面，支持服务器资源监控、软件包批量升级、脚本批量执行等功能。

## 功能特性

- 服务器资源监控（CPU、内存、磁盘）
- 软件包批量升级（支持备份和回滚）
- 脚本批量执行
- 配置文件管理
- 日志检索和查看
- 定时任务管理（crontab可视化）
- 日志轮转和清理配置

## 技术栈

- Python 3.11+
- PyQt6 6.5+
- paramiko 3.4+
- PyInstaller 6.5+

## 快速开始

### 安装依赖

```bash
pip install -r requirements.txt
```

### 运行应用

```bash
python src/main.py
```

### 打包应用

```bash
pyinstaller --onefile --windowed --name=LinuxOpsManager src/main.py
```

## 目录结构

```
LinuxOpsManager/
├── src/              # 源代码目录
│   ├── model/        # 数据模型
│   ├── service/      # 业务服务
│   ├── controller/   # 控制器
│   ├── view/         # 视图组件
│   ├── utils/        # 工具函数
│   └── ui/           # UI资源
├── config/           # 配置文件
├── logs/             # 日志文件
├── tests/            # 测试文件
└── docs/             # 文档
```

## 支持的Linux发行版

- Ubuntu
- 欧拉（openEuler）

## 许可证

MIT License
