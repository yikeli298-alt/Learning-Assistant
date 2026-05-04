---
name: generate-practice
description: 为MSE课程生成练习题，包含详细解析
trigger:
  - "出题"
  - "练习题"
  - "刷题"
  - "生成题目"
  - "practice"
  - "quiz"
---

# MSE 智能出题

## Instructions

When user asks for practice problems:

1. **Clarify requirements** - Ask if not specified:
   - Course and chapter/topic
   - Difficulty level (基础/中等/困难)
   - Number of problems (default: 5)
   - Problem types (选择/计算/分析)

2. **Generate problems**:
   - Match the topic and difficulty
   - Include variety (concept, calculation, application)
   - Mark the knowledge point for each problem

3. **Provide solutions**:
   - Show problems first
   - Then detailed solutions with steps
   - Highlight common mistakes

4. **Keep it focused** - Quality over quantity

5. **Ask follow-up**: "难度合适吗？需要更多题吗？"

## Output Structure

```
# [课程] 练习题 - [知识点]

难度：⭐⭐⭐ (1-5星)

## 题目

**1. [题型]** [题目内容]
[选项/已知条件]

*考点：[知识点]*

---

**2. [题型]** ...

---

## 答案与解析

**1. 答案：[答案]**

解析：
- 关键：[核心概念]
- 步骤：[简要步骤]
- 易错：[常见错误]

**2. 答案：...**
...
```

## Examples

**User**: "出5道材料力学的计算题，关于应力应变"

**Response**:
```
# 材料力学练习题 - 应力应变

难度：⭐⭐⭐

## 题目

**1. 计算题**
一根钢杆，长度 L=2m，横截面积 A=100mm²，弹性模量 E=200GPa。
受拉力 F=20kN 作用。求：
(1) 杆内应力 σ
(2) 杆的伸长量 ΔL

*考点：应力计算、胡克定律*

---

**2. 计算题**
...

---

## 答案与解析

**1. 答案：(1) σ=200MPa  (2) ΔL=2mm**

解析：
- 关键：σ=F/A，ΔL=σL/E
- 步骤：
  (1) σ = 20×10³N / 100×10⁻⁶m² = 200MPa
  (2) ε = σ/E = 200/200000 = 0.001
      ΔL = εL = 0.001×2000 = 2mm
- 易错：单位换算（mm²→m²，GPa→MPa）

需要更多题目或调整难度吗？
```

## Problem Types

**选择题** - Concept understanding, formula application
**计算题** - Numerical problems with clear steps
**分析题** - Mechanism explanation, comparison

## Notes

- Ensure problems are solvable with given information
- Use realistic material properties
- Vary difficulty within the set
- Include at least one "tricky" problem to test deep understanding
