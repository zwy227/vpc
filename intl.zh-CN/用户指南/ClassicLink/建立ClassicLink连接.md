# 建立ClassicLink连接 {#task_xpf_24c_sdb .task}

您可以通过开启ClassicLink功能，建立ClassicLink连接，使经典网络的ECS实例可以和专有网络内的云资源通信。

确保您已经了解建立连接的限制，详情参见[ClassicLink概述](intl.zh-CN/用户指南/ClassicLink/ClassicLink概述.md#)。

1.   登录[专有网络管理控制台](https://vpcnext.console.aliyun.com)。 
2.   选择目标专有网络的地域，然后单击目标专有网络的ID。 
3.   在专有网络详情页面，单击**开启ClassicLink**， 然后在弹出的对话框，单击**确定**。 
4.   登录ECS管理控制台。 
5.   在左侧导航栏，单击**实例**。 
6.   选择实例的所属地域，然后单击目标经典网络ECS实例的**操作**列下的**更多** \> **连接专有网络**。 
7.   在弹出的对话框中选择目标VPC，单击**确定**，然后单击配置安全组的链接。 

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/2441/818_zh-CN.png)

8.   单击**添加ClassicLink安全组规则**，根据以下信息配置ClassicLink安全组规则，然后单击**确定**。 

    |配置|说明|
    |:-|:-|
    |**经典网络安全组**|显示经典网络安全组的名称。|
    |**选择专有网络安全组**|选择专有网络的安全组。|
    |**授权方式**|选择一种授权方式：    -   经典网络 <=\> 专有网络：相互授权访问，推荐使用这种授权方式。
    -   经典网络 =\> 专有网络：授权经典网络ECS访问专有网络内的云资源。
    -   专有网络 =\> 经典网络：授权专有网络ECS访问经典网络ECS。
|
    |**协议类型和端口范围**|选择授权通信的协议和端口。端口的输入格式为xx/xx，比如授权80端口，则输入80/80。|
    |**优先级**|设置该规则的优先级。数字越小，优先级越高。|
    |**描述**|输入安全组描述。|

9.   返回ECS管理控制台，单击右侧的配置图标，在弹出的对话框中勾选**连接状态**，然后单击**确定**查看ECS实例的连接状态。 

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/2441/6557_zh-CN.png "自定义列表选项")

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/2441/6556_zh-CN.png "连接状态选项")

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/2441/819_zh-CN.png "已连接状态")


