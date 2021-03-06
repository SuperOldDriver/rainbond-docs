---
title: 应用状态说明
summary: 应用所有状态说明
toc: false
---

应用一旦创建，就进入到应用的生命周期，在整个生命周期中会有一系列的状态，下文对各个状态进行解释：

|状态 | 说明 | 可进行的操作|
|---- | ---|-------------|
|<font color="#40a9ff">创建中</font> | 新创建的应用，正处于设置阶段 |进行创建流程|
|<font color="#40a9ff">部署中</font> | 新创建的应用设置完成，正在进行第一次应用版本构建 | 重新部署 |
|<font color="#40a9ff">启动中</font> | 应用正在启动，暂时不能访问，启动分为两个阶段，进程启动和业务启动，如果未配置启动时健康检查，只要进程启动完成则认|为应用启动完成| 关闭，重新部署 |
|<font color="#28cb75">运行中</font> | 应用所有运行实例处于运行状态，正常来说处于运行中的应用可以被访问，也可能由于业务启动缓慢应用暂时不能访问|访问，重启，关闭，重新部署|
|<font color="red">运行异常</font> | 应用运行正常的实例少于总实例即标识应用运行异常，对于多实例的应用，处于异常态的应用只要还有正常的实例即可提供服务。<br>实例异常大多数情况是由于应用本身异常退出或因为内存不足发生OOM退出。<br>平台会自动尝试重启异常的实例。|关闭，重启，重新部署|
|<font color="#40a9ff">升级中</font> | 应用正处于滚蛋更新过程中，多个节点处于当前状态的应用可以正常访问 | 关闭|
|已关闭 | 应用已经停止运行，持久化数据依然存在 |启动，重新部署 |
|<font color="#717171">未知</font>  |应用处于此状态可能由于网络受阻，请求后端服务获取应用状态失败，或后端服务异常| |