---
title: "格式指南：查看器压力测试"
description: "包含所有支持模块的单一文档。"
date: "2026-01-24"
tags: ["guide", "format", "viewer"]
author: "ZeroIndex"
type: "post"
---

此文档用于验证帖子查看器的**格式渲染**，包含强调、`代码`、表格和图表等内容。

## 行内样式
- Bold: **bold text**
- Italic: *italic text*
- Strikethrough: ~~deprecated~~
- Inline code: `const answer = 42;`
- Link: [OpenAI](https://openai.com)

## 列表
Unordered:
- First
- Second
  - Nested item

Ordered:
1. Step one
2. Step two
3. Step three

Tasks:
- [x] Completed item
- [ ] Pending item

## 表格
| Feature | Status | Note |
| --- | --- | --- |
| Table scroll | OK | horizontal overflow |
| Code block | OK | syntax highlight |
| Mermaid | OK | svg render |

## 代码块
```ts
type User = {
  id: string;
  name: string;
};

export const greet = (user: User) => {
  return `Hello, ${user.name}!`;
};
```

Long line overflow test:
```
https://example.com/some/really/really/really/really/really/really/really/really/long/path?with=query&and=more
```

Preview card:
```preview
https://example.com
```

## 提示块
:::note title="Note"
This is a note callout with a title.
:::

:::tip title="Tip"
Short tips are highlighted in a friendly tone.
:::

:::warning title="Warning"
Be careful with changes that affect layout.
:::

:::danger title="Danger"
This section flags destructive operations.
:::

:::info title="Info"
Extra context that does not fit inline.
:::

## 折叠内容
:::spoiler summary="Click to reveal"
Hidden content that is revealed on demand.
:::

## Mermaid
```mermaid
graph TD
  A[Start] --> B{Decision}
  B -->|Yes| C[Proceed]
  B -->|No| D[Revise]
```

## 数学
Inline math: $E=mc^2$ and $a^2+b^2=c^2$.

Block math:
$$
\\int_0^\\infty e^{-x} dx = 1
$$

## 图片
![Sample cover](https://placehold.co/1200x600/png)

## 引用
> A calm mind brings inner strength and self-confidence.

## Raw HTML
<div style="padding:12px;border:1px dashed #999;border-radius:12px;background:#faf7f2;">
  Inline HTML block to test rehype-raw.
</div>

## I18n 块
:::i18n id=hero
This block is tagged for synchronized updates across languages.
:::
