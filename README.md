# allkeeper

## 简介

`all` `keepeer` 所有的管理员；

包括但不限于大数据相关组件所有的管理 主要实现对各个组件的运维和监控；

这是一个`文档`类的项目，以文档的形式呈现主要讲解对各组件的运维、监控；

本文档中的操作主要使用`prometheus`+`grafana`实现，后续可能会更新其他老牌监控；

## 项目结构

```
/
├── README.md            项目介绍
├── md-format-mac        对非空目录自动覆盖生成README.md文件并索引当前文件和目录，自动跳过空目录
├── 监控相关              监控生态系统 与 监控指标 相关文档
│   ├── 监控指标
│   └── prometheus生态
└── 运维相关              组件运维的相关文档，运维程序、安装部署等
    ├── hbase
    ├── spark
    ├── zookeeper
    ├── hadoop
    ├── hive
    └── presto
```

## pr提交流程

1. fork项目并在自己的项目中进行clone；
2. 添加原项目的remote地址 `git remote add origin git@github.com:xtdata/allkeeper.git`；
3. 在 `.git/config` 中添加你的github user，主要是名字和邮箱地址，邮箱地址必须与github中的一致；
3. 基于develop分支，创建新的开发分支，【feature/分支名】为日常新功能分支，【fix/分支名】为修复错误分支；
4. 在刚才创建的分支上进行开发；
5. 开发完后，往自己的github中提交；
6. 进去自己的github 项目页面，会有个pr申请，然后进入将代码往原项目的develop分支发起合并申请；


