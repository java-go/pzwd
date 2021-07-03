# 环境监控表[环境监控表](#) <br>### 模型属性本模型相关的参数如<a href="#t2">表2</a>所示。表2 模型参数列表<table id = "t2"><thread><tr><th align = "left">模型参数</th><th align = "left">参数含义</th></tr></thread><tbody><tr><td id = "环境监控编号-1"><a href = "环境监控编号-1.html">环境监控编号</a></td><td></td></tr><tr><td id = "槽位号-2"><a href = "槽位号-2.html">槽位号</a></td><td></td></tr><tr><td id = "环境监控类型-3"><a href = "环境监控类型-3.html">环境监控类型</a></td><td>1：当单板类型是RRU时，2功放温度和3驻波比可选，其他单板类型2和3不可选
2.当单板类型是“FANM”时不支持配置该表；当单板类型是“RRU”时由于rru暂不支持配置，所以暂时不支持配置该表，并且2：功放温度和3：驻波比暂时隐藏；
</td></tr><tr><td id = "环境监控最大值-4"><a href = "环境监控最大值-4.html">环境监控最大值</a></td><td>1.rru 单板温度默认值85
2.射频通道温度默认值100
3.驻波比门限3
4.该字段大于u32EnvMin字段。
5.取值范围：
  1）lte宏站BBU、lte便携式基站MBD和lte小站MBD、车载中心站MCTa和插卡式主备MCTa板范围均为[-40,110]
2）车载中心站BBPa、GES和插卡式BBU的BBPa、PEUa、FSa和ES取值范围均为[-40,85]
6.默认值：
  1)lte宏站BBU、车载中心站除FANM外的所有单板、插卡式BBU除FANM外的所有单板默认值均为70；
  2）lte便携式基站和lte小站的默认值为100。</td></tr><tr><td id = "环境监控最小值-5"><a href = "环境监控最小值-5.html">环境监控最小值</a></td><td>1.该字段小于u32EnvMax字段。
2.取值范围：
  1)同u32EnvMax字段的取值范围。
3.默认值：
  1)lte宏站BBU、车载中心站除FANM外的所有单板、插卡式BBU除FANM外的所有单板默认值均为65；
  2）lte便携式基站和lte小站的默认值为90。</td></tr><tr><td id = "保留字段-6"><a href = "保留字段-6.html">保留字段</a></td><td>1.该字段请在网管和lmt上隐藏。</td></tr></tbody></table>