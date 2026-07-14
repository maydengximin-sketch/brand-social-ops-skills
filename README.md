# Brand Social Ops Skills

一套面向**品牌社交媒体运营**的 AI Agent Skills（10 个），覆盖从品牌社媒总纲、平台流量机制、人群投放、达人筛选、种草战役、数据诊断，到评论区运营、合规审查、高客经营与危机预案的完整链路。

适用于 Claude Code / Claude Agent SDK 及兼容 Agent Skills 规范的环境。

---

## 为什么做这个

品牌方的社媒运营方法论，长期停留在"内部经验"和"外部咨询报告"里，普通创作者、小商家和刚入行的运营几乎接触不到。

但这些东西**并不神秘**——它不难，只是没人系统地写出来。

这个仓库把这套方法论整理成可复用的 skill，让 AI Agent 能直接用它来帮你做判断。

---

## 10 个 Skill

| Skill | 解决什么 |
|---|---|
| [`luxury-social-playbook`](skills/luxury-social-playbook) | 高端品牌社媒总纲：定位、内容支柱、账号矩阵、调性边界 |
| [`kos-program-design`](skills/kos-program-design) | KOS（一线员工）体系：治理、内容模板、激励、线下转化 |
| [`xhs-brand-algorithm`](skills/xhs-brand-algorithm) | 小红书双路流量机制（推荐 / 搜索）与内容对策 |
| [`reverse-funnel-targeting`](skills/reverse-funnel-targeting) | 反漏斗人群模型：从精到泛，小预算撬动效率 |
| [`kol-koc-vetting`](skills/kol-koc-vetting) | 达人筛选、投前数据判读、识别造假、合规接单 |
| [`seeding-campaign-architecture`](skills/seeding-campaign-architecture) | 种草三段式：专业定调 → 口碑铺量 → 搜索占位 |
| [`social-content-metrics`](skills/social-content-metrics) | 数据指标体系与逐层诊断，建立自己的基线 |
| [`comment-section-ops`](skills/comment-section-ops) | 评论区运营、置顶策略、负面分级响应 |
| [`brand-social-compliance`](skills/brand-social-compliance) | 广告标注、违禁词、版权肖像、发布前检查清单 |
| [`luxury-clienteling-events`](skills/luxury-clienteling-events) | 高净值客户分层、活动设计、活动后跟进与 ROI |
| [`social-crisis-playbook`](skills/social-crisis-playbook) | 危机分级、黄金响应时效、声明原则、升级路径 |

> 实际收录 11 个（含危机预案）。

---

## 安装

复制到你的 skills 目录：

```bash
# Claude Code（用户级）
cp -r skills/* ~/.claude/skills/

# 或项目级
cp -r skills/* .claude/skills/
```

每个 skill 是一个独立目录，含 `SKILL.md`（YAML frontmatter + 方法论正文），可单独取用。

---

## 怎么用

安装后直接用自然语言触发，Agent 会自动匹配对应 skill：

- 「我发的笔记一直没流量，帮我看看卡在哪」 → `xhs-brand-algorithm` + `social-content-metrics`
- 「预算不多，这波种草怎么投」 → `reverse-funnel-targeting` + `seeding-campaign-architecture`
- 「这个博主值不值得投」 → `kol-koc-vetting`
- 「这条文案能发吗」 → `brand-social-compliance`
- 「评论区出现负面了怎么办」 → `comment-section-ops` + `social-crisis-playbook`

---

## 内容原则

- **通用方法论，不含任何企业专有信息。** 本仓库全部内容为基于公开行业知识与从业经验的原创总结，不包含、不复述、不衍生自任何公司的内部文件、商业机密、客户数据、第三方付费研究报告或受版权保护的培训材料。
- **不含任何真实品牌、机构或个人的名称与案例数据。**
- **平台机制部分为经验模型**，不是平台官方规则。平台策略持续变化，重要决策前请核验当前官方口径。
- **合规优先。** 所有 skill 均不提供刷量、控评、买粉、水军、规避审核或绕过平台规则的做法；相关内容一律转为风险提示与合规替代方案。
- **不承诺结果。** 不对流量、涨粉、转化或销售做任何保证。

---

## 免责声明

本仓库内容仅供参考与学习，**不构成法律、财务或专业公关意见**。涉及广告合规、知识产权、数据隐私、危机处理等事项，请咨询相应领域的专业人士。

使用者需自行确保其行为符合所在地法律法规及所用平台的当前规则。

---

## License

[MIT](LICENSE)
