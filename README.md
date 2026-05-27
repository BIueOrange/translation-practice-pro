# DualLingo Pro

DualLingo 的升级版，在原有功能基础上增加了账号系统。

## 地址

**[biueorange.github.io/translation-practice-pro](https://biueorange.github.io/translation-practice-pro/)**

## 相比原版新增

- **邮箱登录/注册** — 基于 Supabase Auth，注册后即可登录
- **账号系统** — 支持登录/注册/退出，练习数据可随账号保存

## 功能

- **翻译练习** — 支持中译英和英译中两种模式，显示句子输入翻译后逐词/逐字对比参考答案
- **智能评分** — 基于最长公共子序列 (LCS) 算法计算匹配率，给出 0-100% 评分
- **语法分析** — 自动检测主谓一致、a/an 误用、句首大写、重复词等常见错误
- **题库管理** — 内置 100 句（雅思/四六级/考研/日常/学术），支持增删改、JSON 导入导出
- **练习统计** — 记录每日练习量、时长、连续打卡天数、每周图表、本月练习、练习天数
- **暗色模式** — 手动切换或自动跟随系统

## 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl + Enter` | 提交翻译 |
| `Ctrl + →` | 下一句 |
| `Ctrl + ←` | 上一句 |

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

分类可选值：`ielts`、`cet`、`kaoyan`、`daily`、`academic`

## 技术

纯前端单页应用 + Supabase Auth，无自建后端。
