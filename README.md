# Design of cortexjs.org

By [i@kael.me](mailto:i@kael.me).

![preview](./preview.jpg)


## Search input syntax

```
[<action>:]<param>[|<action>:<param>[|<action>|<param>]]
```

如果 `action` 没有定义，则默认为综合搜索。

#### Search by keywords

```
keywords:dom
```

#### Piped search query

```
keywords:ajax|descend:stars|limit:30
```

按 `package.keywords` 进行搜索，并按照 star 数目降序排序，并仅显示前三个结果


### Available actions

- keywords：按关键字搜索
- name：按名称搜索 