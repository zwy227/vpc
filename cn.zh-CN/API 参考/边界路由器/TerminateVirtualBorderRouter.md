# TerminateVirtualBorderRouter {#reference_i4w_xmt_ndb .reference}

终止边界路由器（VBR）。

调用该接口后VBR从Enabled状态进入Terminated状态，终止成功后进入Terminated状态。在调用本接口终止VBR之前，请注意：

-   只有物理专线的所有者可以调用该接口。

-   VBR进入Terminated状态后，其VLAN ID会保留7天，7天后其他VBR可以使用该VLAN ID。

## 请求参数 {#section_ulr_rpp_vdb .section}

|名称|类型|是否必须|描述|
|:-|:-|:---|:-|
|Action|String|是| 要执行的操作。 取值：

 TerminateVirtualBorderRouter

 |
|RegionId|String|是| VBR所在的地域。

 您可以通过调用 DescribeRegions接口获取地域ID。

 |
|VbrId|String|是| VBR的ID。

 |

## 返回参数 {#section_ugs_f1g_cz .section}

|名称|类型|描述|
|:-|:-|:-|
|RequestId|String|请求ID。|

## 示例 {#section_ix5_h1g_cz .section}

**请求示例**

``` {#createVPCpub}
https://vpc.aliyuncs.com/?Action=TerminateVirtualBorderRouter
&VbrId=pc-2zeoaxkq3xxxxx
&公共请求参数
```

**返回示例**

-   XML格式

    ```
    <?xml version="1.0" encoding="UTF-8"?>
    <TerminateVirtualBorderRouterResponse>
        <RequestId>0ED8D006-F706-4D23-88ED-E11ED28DCAC0</RequestId>
    </TerminateVirtualBorderRouterResponse>
    ```

-   JSON格式

    ```
    { 
        "RequestId": "0ED8D006-F706-4D23-88ED-E11ED28DCAC0"
    }
    ```


