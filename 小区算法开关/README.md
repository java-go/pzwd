# 小区算法开关[小区基本信息](../小区基本信息/README.md) <br>[小区算法开关](#) <br>### 模型描述用于控制CU小区特性的打开和关闭### 创建或删除实例时的生效方式动态生效### 模型关联- 父类： <br>[小区基本信息](../小区基本信息/README.md) <br>- 对象间关联：    - ### 模型属性本模型相关的参数如<a href="#t2">表2</a>所示。表2 模型参数列表<table id = "t2"><thread><tr><th align = "left">模型参数</th><th align = "left">参数含义</th></tr></thread><tbody><tr><td id = "NR小区标识-1"><a href = "NR小区标识-1.html">NR小区标识</a></td><td>该参数用于设置NR小区的标识，在本基站范围唯一标识一个小区。</td></tr><tr><td id = "语音策略开关-2"><a href = "语音策略开关-2.html">语音策略开关</a></td><td>该参数表示5G语音策略控制开关。
EPS_FB_SWITCH(演进数据域回落开关)：该参数用于控制NGRAN语音业务回落E-UTRAN功能开关。</td></tr><tr><td id = "系统间业务移动性算法开关-3"><a href = "系统间业务移动性算法开关-3.html">系统间业务移动性算法开关</a></td><td>该参数用于控制系统间业务移动性的开关。当该开关打开时，启动NG-RAN至EUTRAN系统间业务移动性算法，UE可从NR小区重选/切换/重定向回E-UTRAN系统；当该开关关闭时，关闭NG-RAN至EUTRAN系统间业务移动性算法。</td></tr><tr><td id = " 
异频切换算法开关-4"><a href = " 
异频切换算法开关-4.html"> 
异频切换算法开关</a></td><td> 
该参数主要用来控制系统内异频切换算法的打开和关闭。

COVERAGE_BASED_HO(基于覆盖的异频切换开关)：当基于覆盖的异频切换开关为开时，启动基于覆盖的异频切换算法，通过异频切换保证用户业务连续性；当基于覆盖的异频切换开关为关时，关闭基于覆盖的异频切换算法；
5QI_BASED_REDIRECTION(基于5QI的重定向开关)：当基于5QI的重定向开关为开时，指定5QI将被重定向到配置的频点上；当基于5QI的重定向开关为关时，关闭基于5QI的重定向；
5QI_BASED_HO(基于5QI的异频切换开关)：当基于覆盖的异频切换开关为开时，启动基于覆盖的异频切换算法，通过异频切换保证用户业务连续性；当基于覆盖的异频切换开关为关时，关闭基于覆盖的异频切换算法；
</td></tr><tr><td id = "语音自适应A1 RSRP门限-5"><a href = "语音自适应A1 RSRP门限-5.html">语音自适应A1 RSRP门限</a></td><td>该参数表示语音业务自适应判决的A1事件的RSRP门限。如果服务小区RSRP测量值在时间迟滞内一直高于A1门限时，上报A1事件。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = "INACTIVE策略开关-6"><a href = "INACTIVE策略开关-6.html">INACTIVE策略开关</a></td><td>该参数用于表示RRC INACTIVE态策略控制的开关。
RRC_INACTIVE_SWITCH(RRC INACTIVE开关)：当该开关打开时，启动RRC INACTIVE连接管理，支持RRC CONNECTED和RRC INACTIVE的状态迁移。当该开关关闭时，关闭RRC INACTIVE连接管理。</td></tr><tr><td id = "上行GBR接纳门限-7"><a href = "上行GBR接纳门限-7.html">上行GBR接纳门限</a></td><td>该参数用于表示小区的GBR承载上行接纳的门限，当小区上行GBR速率总和/小区上行峰值速率大于此门限时，将可能触发GBR承载的抢占，抢占失败则接纳失败，当参数配置为100&是表示不进行接纳判断；</td></tr><tr><td id = "下行GBR接纳门限-8"><a href = "下行GBR接纳门限-8.html">下行GBR接纳门限</a></td><td>该参数用于表示小区的GBR承载下行行接纳的门限，当小区上行GBR速率总和/小区上行峰值速率大于此门限时，将可能触发GBR承载的抢占，抢占失败则接纳失败，当参数配置为100&是表示不进行接纳判断；</td></tr><tr><td id = "接纳开关-9"><a href = "接纳开关-9.html">接纳开关</a></td><td>该参数用于表示接纳控制的开关。
GBR_PREEMPT_SWITCH(GBR承载抢占开关):当该开关打开时，GBR承载接纳失败将触发抢占低优先级的GBR承载，会引起低优先级的GBR承载的释放。当该开关关闭时，关闭GBR承载抢占功能。</td></tr><tr><td id = "ROHC头压缩开关-10"><a href = "ROHC头压缩开关-10.html">ROHC头压缩开关</a></td><td>该参数表示ROHC特性开关。
ROHC_SW（ROHC头压缩开关）：该参数用于控制ROHC功能的打开和关闭。当开关打开时，表示ROHC功能启用，还需要配置ROHC Profiles确定最终生效的子协议。当开关关闭时，表示ROHC功能关闭。该参数仅适用于低频。</td></tr><tr><td id = "ROHC子协议开关-11"><a href = "ROHC子协议开关-11.html">ROHC子协议开关</a></td><td>该参数表示ROHC子协议配置。
PROFILE0X0001（子协议0x0001）：主要用于RTP/UDP/IP场景，标准参考RFC 3095，RFC 4815。该参数仅适用于低频。
PROFILE0X0002（子协议0x0002）：主要用于UDP/IP场景，标准参考RFC 3095，RFC 4815。该参数仅适用于低频。</td></tr></tbody></table>