# PowerTools — 汽车调校工程师工具箱

[![Website](https://img.shields.io/badge/Website-ptools.site-blue)](http://ptools.site)
![Language](https://img.shields.io/badge/Language-Python%2FTypeScript-green)

> 专为汽车改装师打造的动力数据分析平台。在线生成马力曲线图、分析CSV数据流、匹配ECU文件、本田ECU在线调校。

## 功能

### 🔧 马力图生成（YourDyno）
- 上传 YourDyno 马力机 CSV 文件，自动生成专业马力/扭矩曲线图
- 自动识别峰值功率（HP）、峰值扭矩（TQ）
- 支持多文件对比、品牌 Logo 定制，Logo 一次上传永久保存
- 专业报告格式：气缸数自动推断、ModSpec 改装清单、燃料类型下拉选择（Gasoline / Diesel / E85 / E50 / E30 / Methanol / Race Gas / Other）
- 曲线平滑度三档可选：关闭 / 标准平滑（峰值偏差 < 0.01%）/ 强力平滑（~0.05%）
- 轮上功率与发动机功率差异分析
- 在线使用，无需安装

### 📈 马力曲线动态分析
- 实时光标跟随：鼠标悬停实时显示对应转速的马力/扭矩值
- 多组曲线叠加对比，每条曲线光标独立跟随
- 拖拽 CSV 即开即用，无需登录
- Dark / Light / Warm 三种图表主题，支持叠加 Logo、导出 PNG
- 移动端自适应

### 📊 CSV 数据流分析
- MHD / Bootmod3 / Autotuner / Ktuner / VCDS 数据流可视化
- **Autotuner 网页端 datalog 链接直连读取**，无需下载 CSV
- 8mb 刷写车型 Datalog CSV 格式支持（含时间戳解析修正）
- WOT 全油门加速段自动识别，图表高亮标注全力加速区间
- 发动机性能面板：最大功率（kW@RPM）、最大扭矩（Nm@RPM）、峰值增压（bar）、爆震总量、加速段次数
- 数据滤波去噪、异常值剔除
- 适用于改装车动力测试数据分析

### 🔍 ECU 文件匹配
- BMW ECU A2L / XDF 文件快速匹配，支持 B48 / B58 / S55 / S58 / S63
- **MHD XDF 匹配工具**：105 个 ECU ID 自动匹配（.bin / .rom 上传，12位精确 + 8位模糊匹配）
- Bosch MED17 / EDC17 / MG1 / MD1 校验和修复
- **XDF → WinOLS JSON 转换工具**：解析全部地图定义，可选上传 BIN 读取实际数值，内置转换验证
- WinOLS NOREAD 数字签名一键擦除

### 🏎 Honda-HEX 本田 ECU 在线调校
- 上传原厂 bin 文件，浏览器内直接修改并下载，纯前端处理
- 自动识别 ECU 版本：八代思域 R18A（10个版本）、飞度 GE8 L15A、三代飞度 GK5 L15B
- 调校功能：点火性能 / MAF 修正 / 破转速 / 踏板响应 / 怠速 / 爆震灵敏度
- L15B 进阶配方：转速表量程、VTEC 介入点、断油点、限速解除、VTC 角度优化、定速巡航激活

### 🛠 调教数据查询
- 59 个品牌、8,000+ 款发动机配置的原厂动力数据
- 覆盖 BMW、Audi、VW、Porsche、Mercedes、Ford、Volvo 及日韩、国产主流品牌
- 原厂马力/扭矩 vs Stage 1 / Stage 2 调校后数据对比
- 部分车型附带 ECU 型号、刷写工具建议和马力机实测曲线图

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
- 本田玩家：原厂 bin 在线调校，无需专业设备

---

*PowerTools — Make your dyno data speak.*
