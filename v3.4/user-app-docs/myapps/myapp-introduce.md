---
title: 应用组管理
summary: 应用组为用户自定义组，组中包含用户创建的各类应用。如用户自定义应用组名为商城应用，该组包含web应用于MySQL 服务。应用组与未分组界面存在差别：应用组界面包括拓扑图以及列表视图，默认以拓扑图展示，可切换至列表视图；未分组只含有列表视图。
toc: false
---
&emsp;&emsp;云帮为了方便您的应用管理，所有应用会以 **应用组** 方式分组。您可以自定义组名称，若未自定义名称，您所创建的应用会默认放至 **未分组** 中。如：用户自定义 **应用组** 包含web应用、MySQL 服务。**应用组** 与 **未分组** 界面存在差别：**应用组** 界面包括**拓扑图**以及**列表视图**，默认以**拓扑图**展示，可切换至**列表视图**；未分组只含有**列表视图**。

<div id="toc"></div>

## 应用组界面

<img src="https://static.goodrain.com/images/acp/docs/user-docs/myapps/myapp-introduce1.png" style="border:1px solid #eee;max-width:100%" />

根据图中序号查看对应解释：

| 序号           | 说明                                    |
| :----------- | :------------------------------------ |
| 1(组名)        | 该组组名，在新增应用时新建或将应用添至已知组                |
| 2(分享)        | 可以把当前的应用分享到云市，并且在**应用市场——分享的应用**中可以看到 |
| 3(管理组)       | 包括修改组名、删除当前组、新增组。删除当前组后组内应用转至未分组中     |
| 4(拓扑图视图)     | 点击当前位置选择拓扑图模式，显示当前组拓扑图(默认显示拓扑图界面)     |
| 5(列表视图)      | 点击当前位置选择列表视图模式，以列表显示当前组所有应用           |
| 6(全屏模式/退出全屏) | 点击实现将拓扑图界面进行全屏模式与退出全屏切换               |
| 7(自定义拓扑图大小)  | 通过滑动原点或点击"➕"、"➖"符号实现对拓扑图的放大与缩小        |

### 拓扑图

<img src="https://static.goodrain.com/images/acp/docs/user-docs/myapps/myapp-introduce2.png" style="border:1px solid #eee;max-width:100%" />

拓扑图视图可以直观的展现出组内应用的连接关系；单击拓扑图上的任意节点（也就是列表视图的应用），可以看到应用名（点击应用名也可进入[应用控制台](myapp-platform-overview.html)）、应用状态、应用分配内存、实例数、服务地址、服务依赖、端口等；拓扑图中单应用名区域会随着应用状态的变更而变化，开启状态为绿色，关闭状态为红色。

### 列表

<img src="https://static.goodrain.com/images/acp/docs/user-docs/myapps/myapp-introduce3.png" style="border:1px solid #eee;max-width:100%" />

| 序号       | 说明                                      |
| -------- | --------------------------------------- |
| 1(应用名)   | 点击应用名进入对应应用                             |
| 2(操作)    | 实现对单个应用的启动与关闭操作                         |
| 3(批量操作台) | 通过左侧的复选框选择多个应用，实现对多个应用的批量启动、批量重新部署、批量关闭 |

## 未分组界面

<img src="https://static.goodrain.com/images/acp/docs/user-docs/myapps/myapp-introduce4.png" style="border:1px solid #eee;max-width:100%" />

未分组视图操作与**分组视图-列表**基本相同