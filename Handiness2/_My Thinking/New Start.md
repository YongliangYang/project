﻿

### 运行起始

SchemaBootmgr 引导框架加载所有的 Schema 信息


### Lambda 表达式解析与链式调用

1.类似于 (#1) Select(t=>new {t.Name,t.Age}) 的表达式，此类表达式目的在于过滤获取的信息，此表达式类型为 NewExpression

这里我们为了将表达式转换为 SQL 需要获取与传入参数类型关联的元数据信息（获取表名等），以及所使用属性上的元数据信息（获取列名等）
例如 （#1） 所示的表达式，最后可能转换为  "[a].[name],[a].[age]"

2.

