# 介绍文档
官方 jaeger 的本地 fork, 修复了:

1. uuid 支持 - 查询

## 编译
**注意: 编译 build-query 前, 需要首先 编译 build-ui**

由于本项目目前一直采用vendor编译方式, 需要按以下过程编译

### 环境准备
1. 安装 go 环境
2. 安装 git
3. 安装 dep: go get -u github.com/golang/dep/cmd/dep, 并将 dep 放到可执行路径下

### 编译准备
1. mkdir -p $GOPATH/src/github.com/jaegertracing
2. cd $GOPATH/src/github.com/jaegertracing
3. git clone git@github.com:jaegertracing/jaeger.git jaeger
4. cd jaeger
5. git submodule update --init --recursive
6. dep ensure
7. make install-tools

### 编译
1. make build-agent ...