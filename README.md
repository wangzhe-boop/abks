# ABKS 商务工作台

> 达人寄样全链路管理工具 —— 面向抖音达人对接与企业微信商务协作的线上化工作台。

[![Pages](https://img.shields.io/badge/GitHub%20Pages-已部署-1f6feb)](https://wangzhe-boop.github.io/abks/)
[![Issues](https://img.shields.io/github/issues/wangzhe-boop/abks)](https://github.com/wangzhe-boop/abks/issues)

## 简介

单文件 HTML 应用（无需构建、双击即开），覆盖 **商务 / 达人 / 寄样** 三大核心场景：

- **寄样管理**：寄样子表单（编码 / 贺卡 / 视频）、多次寄样、定时催样、寄样全流程流水线（绑定→寄样→分享码→催跟→合作完成，含 45 天未完成判定）
- **达人管理**：达人字段排序、待办角标、蝉圈圈任务绑定、列表待办智能排序
- **投流申请**：两列投流申请字段
- **抖音智能识别**：达人主页智能识别录入
- **云端同步**：接入 Supabase 实现云端登录与数据同步，支持本地离线后在网络恢复自动上传

## 功能截图

> 以下为各模块截图占位，后续版本将替换为真实界面截图。

| 模块 | 截图占位 |
|------|----------|
| 工作台首页 / KPI 看板 | `（截图占位）首页 KPI 卡片 + 7 天趋势图` |
| 寄样全流程流水线 | `（截图占位）绑定 → 寄样 → 分享码 → 催跟 → 合作完成` |
| 达人管理列表 | `（截图占位）达人字段排序 + 待办角标` |
| 投流申请 | `（截图占位）两列投流申请字段` |
| 抖音智能识别 | `（截图占位）达人主页智能识别录入` |

## 快速开始

本工具为**纯前端单文件应用**，无需安装依赖、无需构建：

1. 下载或克隆本仓库：
   ```bash
   git clone https://github.com/wangzhe-boop/abks.git
   cd abks
   ```
2. 直接用浏览器打开主程序文件即可使用：
   - 主程序：`ABKS商务工作台.html`（双击或拖入浏览器）
   - 在线版（GitHub Pages 自动部署）：<https://wangzhe-boop.github.io/abks/>
   - 内部在线版入口（随版本更新）：<https://d3551080f2894b6280bfb6e1a2fed312.app.workbuddy.link>

> Tips：首次使用建议在浏览器中允许本地存储，以便离线缓存数据；联网后会通过 Supabase 自动同步到云端。

## 技术栈

- **前端**：原生 JavaScript（Vanilla JS），单文件 HTML 架构，无框架、无构建步骤
- **数据存储与同步**：[Supabase](https://supabase.com/)（Postgres + Auth + Realtime），支持云端登录、数据同步与本地离线缓存
- **部署**：GitHub Pages（分支部署 + GitHub Actions 自动部署）
- **协作**：GitHub Issues + Projects 管理需求与迭代看板

## 目录说明

- `ABKS商务工作台.html` —— 生产主程序（当前版本）
- `index.html` —— GitHub Pages 入口（与主程序同源，用于静态站点部署）
- `*.html.v*_baseline_*` —— 各版本冻结基线快照（只增不改，用于回滚）
- `ABKS商务工作台-*-原型.html` —— 迭代工作副本

## 迭代约定

每次迭代在生产主文件冻结基线后，于工作副本改动并自测，确认后再合入；所有改动均保留基线快照以便回溯。

## 作者

**ABKS 团队** · 抖音达人商务协作方向

- GitHub：[@wangzhe-boop](https://github.com/wangzhe-boop)
- 仓库：<https://github.com/wangzhe-boop/abks>

---

© ABKS. 达人寄样全链路管理工具。
