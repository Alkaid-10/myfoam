# SelectionDAG
`DAG`(有向无环图):LLVM代码生成器用来表示各种操作，连同它们所产生及消耗值的一种数据结构
`SelectionDAG`是一种trees-on-DAGs的有向图覆盖实现, 编译器开发人员通过编写指令的树匹配(tree pattern), 通过`tablgen`翻译成完整的树匹配代码交由代码生成器(matcher generator)处理, 后者采用贪婪的DAG-to-DAG策略将中端IR覆写为机器指令描述.