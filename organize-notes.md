---
name: organize-notes
description: 整理MSE课程笔记，构建结构化知识体系
trigger:
  - "整理笔记"
  - "笔记整理"
  - "课后整理"
  - "organize notes"
  - "梳理知识点"
---

# MSE 笔记整理

## Instructions

When user provides class notes or asks to organize notes:

1. **Identify course and chapter** - Ask if not clear
2. **Extract key elements**:
   - Core concepts and definitions
   - Important formulas
   - Key principles and mechanisms
3. **Structure hierarchically**:
   - Chapter → Topics → Sub-concepts
   - Mark: 重点 / 难点 / 易错点
4. **Keep it concise** - Focus on essentials, not exhaustive details
5. **Ask follow-up**: "需要补充例题吗？" or "哪部分需要展开？"

## Output Structure

Use this structure, but **adapt to content** (don't force all sections):

```
# [课程名] - [章节名]

## 核心概念

### [概念1]
- 定义：[简洁定义]
- 公式：$...$（如有）
- 关键点：[2-3个要点]

### [概念2]
...

## 知识关联
[概念A] → [概念B] → [应用]

## 重点标注
- ⚠️ 易错：[常见错误]
- 🔥 必考：[高频考点]
- 💡 技巧：[记忆方法]

## 例题（可选）
[如果笔记中有例题，简要整理]
```

## Examples

**User**: "帮我整理材料力学第三章的笔记：应力应变关系，胡克定律..."

**Response**:
```
# 材料力学 - 第3章 应力应变

## 核心概念

### 应力 (Stress)
- 定义：单位面积上的内力，$\sigma = F/A$
- 类型：正应力（拉/压）、切应力
- 单位：Pa, MPa

### 应变 (Strain)  
- 定义：相对变形，$\epsilon = \Delta L / L_0$
- 无量纲

### 胡克定律
- 线弹性范围：$\sigma = E\epsilon$
- E = 弹性模量（材料常数）
- 适用条件：小变形 + 弹性范围

## 知识关联
应力 + 应变 → 胡克定律 → 弹性模量测定

## 重点标注
- ⚠️ 易错：应力有方向性，应变是标量
- 🔥 必考：胡克定律适用条件
- 💡 技巧：E 越大越"硬"（抗变形能力强）

需要补充例题吗？
```

## Notes

- Prioritize clarity over completeness
- Use LaTeX for formulas: `$\sigma = E\epsilon$`
- If notes are messy, help reorganize logically
- Suggest related concepts from other chapters if relevant
