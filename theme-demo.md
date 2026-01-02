# 一级标题 / H1

## 二级标题 / H2

### 三级标题 / H3

#### 四级标题 / H4

##### 五级标题 / H5

###### 六级标题 / H6

# Theme Demo

## 1. 文本 / Text

这是一段正文内容样式，以下是不同文本样式效果：**这是加粗文本样式**，<u>这是下划线样式</u>，*这是斜体字样式*，[这是超链接](https://github.com/)，`This is a single line code style`，~~这是删除线效果样式~~，==这是文字高亮效果==，上下标样式：$\LaTeX$，X^2^，H~2~O，键盘键样式：<kbd>Command+Q</kbd>，以及 emoji：🐳 😀 🌟

This is a text content style and the following are the effects of different text styles: **This is a bold text style**, [This is a hyperlink style](https://github.com), *This is the italic font style*, ~~This is the strikethrough effect style~~, <u>This is the underline style</u>, `This is a single line code style`, keyboard key style: <kbd>Command+Q</kbd>, $\LaTeX$ X^2^ H~2~O, ==This is the text highlighting effect==, 🐳 😀 🌟

> 一段引用文本
> A blockquote for testing.

---

## 2. 代码块 / Code Blocks

单行代码样式 / Inline code：`README`

```python
import os
from openai import OpenAI

client = OpenAI(api_key=os.environ.get("OPENAI_API_KEY"))

resp = client.chat.completions.create(
    model="gpt-4o-mini",
    messages=[
        {"role": "system", "content": "You are a helpful assistant."},
        {"role": "user", "content": "Write a haiku about Hokkaido."},
    ],
)

print(resp.choices[0].message.content)
```

---

## 3. 数学公式 / Math

设数据样本 $x_0\sim q(x_0)$，扩散模型的前向过程逐步加入高斯噪声：

$$
q(x_t \mid x_{t-1})=\mathcal N\bigl(x_t;\sqrt{1-\beta_t}\,x_{t-1},\,\beta_t\mathbf I\bigr),\quad t=1,\dots,T
$$

## 4. 引用与警示框 / Blockquotes & Alerts

> 单层引用：读书破万卷，下笔如有神。  
> Single quote: “Read ten thousand books, write as if inspired.”

> 多层引用 / Nested:
> > 二级引用 / Level 2
> > > 三级引用 / Level 3

> [!NOTE]
>
> This is a Note text box ...... `this is code style`

> [!TIP]
>
> - This is a Tip text box ......

> [!IMPORTANT]
>
> This is a Important text box ......

> [!WARNING]
>
> This is a Warning text box ......

> [!CAUTION]
>
> This is a Caution text box ......

---

## 5. 列表 / Lists

### 5.1 无序列表 / Unordered

- 苹果 / Apple
- 香蕉 / Banana
  - 青香蕉 / Green banana
  - 熟香蕉 / Ripe banana
- 樱桃 / Cherry

### 5.2 有序列表 / Ordered

1. 第一步 / Step one
2. 第二步 / Step two
3. 第三步 / Step three

### 5.3 任务列表 / Task Lists

- [ ] 待办事项 / Todo item
- [x] 已完成事项 / Done item
- [ ] 另一个任务 / Another task

---

## 6. 表格 / Tables

| 项目 / Item | 数量 / Qty | 备注 / Note |
|:-:|:--:|:--:|
| 铅笔 / Pencil | 2 | HB |
| 橡皮 / Eraser | 1 | 白色 / White |
| 笔记本 / Notebook | 3 | A5 |

---

## 7. 图表 / Diagrams

```mermaid
flowchart LR
  A[开始 / Start] --> B{判断 / Decide}
  B -->|是 / Yes| C[执行 / Do]
  B -->|否 / No| D[结束 / End]
```

```mermaid
sequenceDiagram
  participant U as 用户 / User
  participant A as 应用 / App
  U->>A: 打开文件 / Open file
  A-->>U: 渲染主题 / Render theme
```
