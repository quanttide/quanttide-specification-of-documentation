# 作者

本文定义“主要作者”（Author）和“合著者”（Coauthor）。

## 领域模型定义

- 主要作者（Author）：对文章内容做出主要贡献的一个或者多个人。
- 合著者（Coauthor）：对

## Metadata字段规则

### 字段定义

- `author`: 单个主要作者，值为字符串。
- `authors`: 多个主要作者，值为数组。
- `coauthor`: 单个合著者，值为字符串。
- `coauthors`: 多个合著者，值为数组

### 约束

- `author`和`authors`不可以同时存在，`coauthor`和`coauthors`不可以同时存在。
- `coauthor`或者`coauthors`不可以单独存在，必须要有`author`或者`authors`存在。

## 最佳实践

### 单个主要作者

```yaml
---
author: 张三
---
```

### 单个主要作者和合著者

常见于：

- 一个人主要创作、其他人协助修改。

```yaml
---
author: 张三
coauthor: 李四
---
```

### 多个主要作者

常见于：

- 多个人同时创作一个稿子。
- 下一个人在上一个人的基础上重写稿子。此时常见实践是把`author`字段改为`authors`字段。

```yaml
authors:
  - 张三
  - 李四
```

### 多个主要作者和合著者

```yaml
authors:
  - 张三
  - 李四
coauthors:
  - 王五
  - 赵小二
```
