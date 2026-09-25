# 古籍与历史案例决策推演

一个可在 Codex、WorkBuddy 等兼容 Agent Skills 的工具中使用的技能。它从你指定的书本库检索决策机制相似的案例，重建当时的选项判断、结果和显性/隐性代价，标注可复查出处，再推演规律、现实启发与风险边界。

技能只包含分析流程，不包含《资治通鉴》《毛泽东选集》《史记》等书的全文。使用时需要提供可访问的书库、文件或检索入口；技能会明确区分原文证据、分析推断和面向当前问题的推演。

## 在 WorkBuddy 中安装

1. 下载 [`dist/life-decision-from-books.zip`](dist/life-decision-from-books.zip)。
2. 在 WorkBuddy 打开“专家·技能·连接器”中的“技能”，选择“添加技能”并导入本地技能包。
3. 安装后，在决策问题中提供书库位置或相关文本，并说明当前选项、约束和优先级。

WorkBuddy 技能结构与导入说明见[官方文档](https://open.workbuddy.cn/docs/skill)。

## 在 Codex 中安装

将 [`skills/life-decision-from-books`](skills/life-decision-from-books) 目录复制到 `~/.codex/skills/`，之后可在请求中使用 `$life-decision-from-books`，也可由 Codex 根据请求自动调用。
