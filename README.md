# 介绍文档
官方 jaeger 的本地 fork, 修复了:

1. uuid 支持 - 查询

## 编译

请参考文档: ![编译文档](./CONTRIBUTING.md)

注意: 编译 build-query 前, 需要首先 编译 build-ui

注意: metrics 编译, 首先需要 clone https://git.sysop.bigo.sg/dev-tools/tracing, 并将下层目录 metrics, ln -s 到 cmd 目录内
