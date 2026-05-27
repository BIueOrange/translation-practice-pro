# 中译英翻译练习

一个浏览器即开即用的中译英翻译练习工具，适合雅思、四六级等英语考试备考。

## 地址

**[biueorange.github.io/translation-practice](https://biueorange.github.io/translation-practice/)**

电脑和手机浏览器均可使用，无需下载安装。

## 功能

- **翻译练习** — 显示中文句子，输入英文翻译，提交后逐词对比参考答案
- **智能评分** — 基于最长公共子序列 (LCS) 算法计算词级匹配率，给出 0-100% 评分
- **语法分析** — 自动检测主谓一致、a/an 误用、句首大写、重复词等常见错误
- **题库管理** — 内置 80 句（雅思/四六级/日常/学术），支持增删改、JSON 导入导出
- **练习统计** — 记录每日练习量、时长、连续打卡天数、每周图表
- **暗色模式** — 手动切换或自动跟随系统

## 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl + Enter` | 提交翻译 |
| `Ctrl + →` | 下一句 |
| `Ctrl + ←` | 上一句 |

## 本地使用

1. 下载 `index.html`
2. 双击用浏览器打开
3. 所有数据保存在浏览器本地存储中，无需网络

## 题库格式

导入 JSON 时使用以下格式：

```json
[
  {
    "chinese": "随着科技的发展，人们的生活方式发生了变化。",
    "english": "With the development of technology, people's lifestyles have changed.",
    "category": "ielts"
  }
]
```

分类可选值：`ielts`、`cet`、`daily`、`academic`

## 技术

纯前端单页应用，无框架依赖，无网络请求，数据存储在 localStorage。
