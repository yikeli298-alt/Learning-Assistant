---
name: study-session
description: 完整的MSE学习工作流，从预习到复习的全流程支持
trigger:
  - "开始学习"
  - "学习计划"
  - "复习计划"
  - "study plan"
  - "备考"
---

# MSE 学习流程

## Instructions

When user wants to start a study session or create a study plan:

1. **Understand the goal**:
   - New chapter (预习 + 学习)
   - Review for exam (系统复习)
   - Practice session (刷题巩固)

2. **Create a focused plan**:
   - Set clear objectives (3-5 items)
   - Break into manageable steps
   - Estimate time for each step

3. **Guide through stages**:
   - **预习**: Overview key concepts
   - **学习**: Deep dive (use `explain-concept` if needed)
   - **整理**: Structure notes (suggest `organize-notes`)
   - **练习**: Generate problems (suggest `generate-practice`)
   - **复习**: Review and reinforce

4. **Track progress** - Use checkboxes, update as user progresses

5. **Keep it actionable** - Specific next steps, not generic advice

## Output Structure

```
# 学习计划：[课程] - [章节/目标]

## 目标
- [ ] [具体目标1]
- [ ] [具体目标2]
- [ ] [具体目标3]

## 学习路径

### 第1步：[阶段名] (预计XX分钟)
[具体要做什么]

### 第2步：[阶段名] (预计XX分钟)
[具体要做什么]

### 第3步：...

## 当前阶段
📍 [当前在哪一步]

## 下一步行动
[明确的下一步指令]
```

## Examples

**User**: "我要开始学习材料力学第4章"

**Response**:
```
# 学习计划：材料力学 - 第4章 扭转

## 目标
- [ ] 理解扭转变形的基本概念
- [ ] 掌握扭转应力和应变计算
- [ ] 能够分析圆轴扭转问题

## 学习路径

### 第1步：预习 (15分钟)
- 浏览章节大纲
- 识别核心公式：τ=Tr/Ip, φ=TL/GIp
- 标注疑问点

### 第2步：深入学习 (30分钟)
- 理解扭矩、切应力、扭转角的关系
- 推导公式（我可以帮你解释）
- 记录重点

### 第3步：整理笔记 (20分钟)
说"整理笔记"，我帮你结构化整理

### 第4步：练习巩固 (30分钟)
说"出5道扭转的计算题"，开始刷题

## 当前阶段
📍 第1步：预习

## 下一步行动
先浏览教材第4章，然后告诉我有哪些不理解的概念，我来详细解释。
```

## Notes

- Adapt plan to user's available time
- Suggest other skills when appropriate (but don't force)
- Be flexible - user may skip or reorder steps
- Focus on one chapter/topic at a time
