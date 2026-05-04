---
name: exam-prep
description: 考前冲刺系统，快速复习和模拟考试
trigger:
  - "考试"
  - "考前冲刺"
  - "模拟考试"
  - "exam prep"
  - "期末复习"
---

# MSE 考前冲刺

## Instructions

When user is preparing for an exam:

1. **Assess the situation**:
   - How much time until exam? (1天/3天/1周)
   - Exam scope (chapters, topics)
   - User's weak points (if known)

2. **Choose the mode**:
   - **快速复习模式** (1-3天): Core concepts + formulas + common mistakes
   - **模拟考试模式** (有时间): Generate mock exam + grading

3. **Prioritize ruthlessly**:
   - Focus on high-frequency topics
   - Skip low-yield details
   - Emphasize common mistakes

4. **Keep it concise** - Exam prep is about efficiency, not completeness

5. **Provide actionable tips** - What to review tonight, what to memorize

## Output Structure

### 快速复习模式

```
# 考前冲刺：[课程]

## 必背公式 (5分钟速记)
1. **[公式名]**: $...$
   - 适用：[条件]
   - 常考：[题型]

## 核心概念 (一句话版)
- **[概念]**: [最简定义]
- **[概念]**: [最简定义]

## 高频考点
1. [考点] - [为什么常考]
2. [考点] - [为什么常考]

## 易错清单
1. **[易错点]**
   ❌ 错误：...
   ✅ 正确：...

## 考前建议
- 今晚重点看：[具体内容]
- 明早再过一遍：[具体内容]
```

### 模拟考试模式

```
# 模拟试卷：[课程]

时间：XX分钟 | 总分：100分

## 一、选择题 (XX分)
[题目]

## 二、计算题 (XX分)
[题目]

## 三、分析题 (XX分)
[题目]

---

# 参考答案
[详细答案 + 评分标准]
```

## Examples

**User**: "材料力学期末考试，后天考，帮我冲刺一下"

**Response**:
```
# 考前冲刺：材料力学

时间紧，聚焦高频考点！

## 必背公式 (5分钟速记)

1. **胡克定律**: $\sigma = E\epsilon$
   - 适用：线弹性、小变形
   - 常考：给E和ε求σ

2. **扭转切应力**: $\tau = \frac{Tr}{I_p}$
   - 适用：圆轴扭转
   - 常考：强度校核

3. **弯曲正应力**: $\sigma = \frac{My}{I_z}$
   - 适用：纯弯曲
   - 常考：最大应力位置

## 高频考点 (必考！)

1. **轴向拉压** - 应力应变计算 (每年必考)
2. **扭转** - 强度和刚度校核 (80%概率)
3. **弯曲** - 剪力图弯矩图 (必考大题)

## 易错清单

1. **单位换算**
   ❌ 错误：MPa 和 Pa 混用
   ✅ 正确：1 MPa = 10⁶ Pa

2. **符号正负**
   ❌ 错误：拉应力为负
   ✅ 正确：拉应力为正，压应力为负

3. **截面惯性矩**
   ❌ 错误：圆形 I = πd⁴/64
   ✅ 正确：圆形 I = πd⁴/64 (直径), I = πr⁴/4 (半径)

## 今晚行动计划

1. **19:00-20:00**: 过一遍所有公式，默写3遍
2. **20:00-21:30**: 刷10道计算题（拉压+扭转+弯曲各3题）
3. **21:30-22:00**: 看错题本，重点看易错点

需要模拟试卷吗？说"生成模拟试卷"。
```

## Notes

- Time-sensitive: adapt to days remaining
- Be realistic about what can be covered
- Prioritize understanding over memorization (but formulas must be memorized)
- Encourage sleep before exam (don't cram all night)
