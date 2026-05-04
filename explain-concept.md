---
name: explain-concept
description: 深入解释MSE概念，用类比和例子帮助理解
trigger:
  - "解释"
  - "什么是"
  - "为什么"
  - "怎么理解"
  - "explain"
  - "what is"
---

# MSE 概念解析

## Instructions

When user asks about an MSE concept:

1. **Identify the concept** and user's confusion point
2. **Explain in layers** (simple → detailed):
   - One-sentence core definition
   - Everyday analogy
   - Professional definition with formula (if applicable)
   - Underlying mechanism (if user needs depth)
3. **Provide context**:
   - Related concepts
   - Common applications
   - Typical mistakes
4. **Keep it concise** - expand only if user asks for more detail
5. **Ask follow-up**: "需要例题吗？" or "哪部分需要更详细？"

## Output Structure

Use this structure, but **keep each section brief** (2-3 sentences unless user asks for more):

```
# [概念名称]

## 核心定义
[一句话 + 公式（如有）]

## 通俗理解
[类比例子]

## 专业解释
[学术定义 + 物理意义]

## 常见误区（如有）
[易错点对比]

## 相关概念
[前置/相关知识点]
```

## Examples

**User**: "解释一下位错"
**Response**: 
```
# 位错 (Dislocation)

## 核心定义
晶体中原子排列的线缺陷，导致局部应力集中。

## 通俗理解
想象一排整齐的砖墙，中间插入半排砖，边界就是位错线。

## 专业解释
- **刃位错**：多余半原子面的边界
- **螺位错**：原子面螺旋排列
- **柏氏矢量** b 描述位错强度和方向

## 为什么重要
- 控制材料塑性变形
- 影响强度和韧性
- 位错运动 = 材料变形

需要看位错运动的例题吗？
```

## Notes

- Adapt depth to user's level (基础/进阶)
- Use LaTeX for formulas: `$\sigma = E\epsilon$`
- Prioritize understanding over completeness
- If concept is complex, break into sub-questions
