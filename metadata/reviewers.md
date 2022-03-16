# 审稿人

## 领域模型定义

审稿人（Reviewers），指对稿子提出修改意见的人。
通常和主要作者不是同一批人、可以通过合著者的形式协助作者修改文章。

## Metadata字段定义

### 字段定义

`reviewers`: 值为数组

### 字段约束

`reviewers`的成员不可以和`author`、`authors`等主要作者字段重复、允许和`coauthors`的值重复。

## 最佳实践

```yaml
---
author: 张三
coauthors:
  - 李四
reviewers:
  - 李四
  - 王五
---
```

上述含义为：张三是主要作者，李四和王五审稿，李四顺便帮王五修改了一些内容。
