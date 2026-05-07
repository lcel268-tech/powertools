# PowerTools — 汽车调校工程师工具箱

[![Website](https://img.shields.io/badge/Website-ptools.site-blue)](http://ptools.site)
![Language](https://img.shields.io/badge/Language-Python%2FTypeScript-green)

> 专为汽车改装师打造的动力数据分析平台。在线生成马力曲线图、分析CSV数据流、匹配ECU文件。

## 功能

### 🔧 马力图生成（YourDyno）
- 上传 YourDyno 马力机 CSV 文件，自动生成专业马力/扭矩曲线图
- 自动识别峰值功率（HP）、峰值扭矩（TQ）
- 支持多文件对比、品牌 Logo 定制
- 轮上功率与发动机功率差异分析
- 在线使用，无需安装

### 📊 CSV 数据流分析
- MHD / Bootmod3 / Autotuner / Ktuner / VCDS 数据流可视化
- 数据滤波去噪、异常值剔除
- 适用于改装车动力测试数据分析

### 🔍 ECU 文件匹配
- BMW ECU A2L / XDF 文件快速匹配
- Bosch MED17 / EDC17 / MG1 / MD1 校验和修复
- XDF → WinOLS JSON 格式转换
- WinOLS NOREAD 数字签名去除

### 🛠 调教数据查询
- 5000+ 车型调教数据
- 覆盖 BMW、Audi、VW、Porsche、Mercedes 等主流品牌
- 原厂马力/扭矩 vs 调校后数据对比

## 快速开始

访问 [ptools.site](http://ptools.site) 即可使用，无需注册。
提供 Demo 账号，5 分钟上手。

## 技术栈

| 组件 | 技术 |
|------|------|
| 前端 | Next.js / TypeScript / Canvas |
| 后端 | Python Flask |
| 工具链 | rx14-cli (C++), OpenCLI |
| 数据 | 飞书多维表格, JSON |

## 链接

- 网站: [ptools.site](http://ptools.site)
- 更新日志: [/updates](https://ptools.site/updates)

## 适用场景

- 改装店技师：快速生成客户马力测试报告
- ECU 调校工程师：数据分析与文件匹配
- 车队管理者：多车动力数据对比与存档

---

*PowerTools — Make your dyno data speak.*
