# 项目配置`_config.yml`

遵循[Jupyter Book的`config.yml`文件规范](https://jupyterbook.org/en/stable/customize/config.html)。

此外，额外规范下述字段。

## 名称`name`

用户指定的唯一标识。用于生成URL(i.e. `/courses/{course_name}`)等面向用户的唯一性标识。

## 标题`title`

必填。同Jupyter Book。

## 作者`author`

必填。同Jupyter Book。

所属量潮科技的文档默认署名为`量潮科技`。

## 描述`description`

项目描述。

## 分类`category`

文档规范的子类型，不同的子类型根据需要拓展必要实现。

可选：

- `doc`: 文档。默认类型。
- `tutorial`: 教程。主要用于量潮课堂的教程项目。

## 标签`tags`

数组格式。标记所属知识领域。

## 研发阶段`stage`

标记项目的研发周期所属阶段。

可选：

- `dev`
- `alpha`
- `beta`
- `rc`
- `release`

## 难度`level`

教程类型必选。标记知识水平。

可选:

- `introductory`: 初级。
- `intermediate`: 中级。
- `advanced`: 高级。
