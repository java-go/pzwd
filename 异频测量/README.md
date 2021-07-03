# 异频测量[小区基本信息](../小区基本信息/README.md) <br>[异频测量](#) <br>### 模型描述用于配置系统内的异频切换测量参数，针对不同的QCI提供不同的切换参数，满足不同的业务对目标小区的不同要求。### 创建或删除实例时的生效方式动态生效### 模型关联- 父类： <br>[小区基本信息](../小区基本信息/README.md) <br>- 对象间关联：    - 创建CU小区时，系统默认创建"InterFreqHoMeasGroupId"为0的配置### 模型属性本模型相关的参数如<a href="#t2">表2</a>所示。表2 模型参数列表<table id = "t2"><thread><tr><th align = "left">模型参数</th><th align = "left">参数含义</th></tr></thread><tbody><tr><td id = "NR小区标识-1"><a href = "NR小区标识-1.html">NR小区标识</a></td><td>该参数表示NR小区的标识，在本基站范围内唯一标识一个小区。</td></tr><tr><td id = " 
异频切换测量参数组标识-2"><a href = " 
异频切换测量参数组标识-2.html"> 
异频切换测量参数组标识</a></td><td> 
该参数表示异频切换测量参数组标识。</td></tr><tr><td id = " 
异频A4A5幅度迟滞-3"><a href = " 
异频A4A5幅度迟滞-3.html"> 
异频A4A5幅度迟滞</a></td><td>该参数表示异频A4A5事件的幅度迟滞，用于减少由于无线信号波动导致的对小区切换测量的频繁解除和触发，减少乒乓切换和误判，该值越大越容易防止乒乓和误判。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = "异频A1A2时间迟滞-4"><a href = "异频A1A2时间迟滞-4.html">异频A1A2时间迟滞</a></td><td>该参数表示异频A1A2事件的时间迟滞，当A1A2事件满足触发条件时并不立即上报，而是当该事件在时间迟滞内，一直满足触发门限，才触发上报该事件测量报告。参数的使用细节参见3GPP TS 38.331。

是否主键 
否</td></tr><tr><td id = "异频A1A2幅度迟滞-5"><a href = "异频A1A2幅度迟滞-5.html">异频A1A2幅度迟滞</a></td><td>该参数表示异频A1A2事件的幅度迟滞，用于减少由于无线信号波动导致的对小区切换测量的频繁解除和触发，减少乒乓切换和误判，该值越大越容易防止乒乓和误判。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
异频A4A5时间迟滞-6"><a href = " 
异频A4A5时间迟滞-6.html"> 
异频A4A5时间迟滞</a></td><td> 
该参数表示异频A4A5事件的时间迟滞，当A4A5事件满足触发条件时并不立即上报，而是当该事件在时间迟滞内，一直满足触发门限，才触发上报该事件测量报告。该参数可以减少偶然性触发的事件上报，并降低平均切换次数和误切换次数，防止不必要切换的发生。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A5 RSRP触发门限1-7"><a href = " 
基于覆盖的异频A5 RSRP触发门限1-7.html"> 
基于覆盖的异频A5 RSRP触发门限1</a></td><td>该参数表示基于覆盖的异频切换的A5事件的本服务小区RSRP门限1。如果服务小区RSRP测量值在异频A4A5时间迟滞InterFreqA4A5TimeToTrig内一直低于此门限，且邻区信号质量高于门限CovInterFreqA5RsrpThld2，UE将上报A5事件。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A5 RSRP触发门限2-8"><a href = " 
基于覆盖的异频A5 RSRP触发门限2-8.html"> 
基于覆盖的异频A5 RSRP触发门限2</a></td><td> 
该参数表示基于覆盖的异频切换的A5事件的邻区RSRP门限2。如果服务小区RSRP测量值在异频A4A5时间迟滞InterFreqA4A5TimeToTrig内一直低于门限CovInterFreqA5RsrpThld1，且邻区信号质量高于此门限，UE将上报A5事件。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A2 RSRP触发门限-9"><a href = " 
基于覆盖的异频A2 RSRP触发门限-9.html"> 
基于覆盖的异频A2 RSRP触发门限</a></td><td>该参数表示基于覆盖的异频切换A2 RSRP触发门限。如果服务小区RSRP测量值在异频A1A2时间迟滞InterFreqA1A2TimeToTrig内一直低于该门限，将上报A2测量报告。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A1 RSRP触发门限-10"><a href = " 
基于覆盖的异频A1 RSRP触发门限-10.html"> 
基于覆盖的异频A1 RSRP触发门限</a></td><td> 
该参数表示基于覆盖的异频切换A1 RSRP触发门限。如果服务小区RSRP测量值在异频A1A2时间迟滞InterFreqA1A2TimeToTrig内一直超过该门限，将上报A1测量报告。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A5 SINR触发门限1-11"><a href = " 
基于覆盖的异频A5 SINR触发门限1-11.html"> 
基于覆盖的异频A5 SINR触发门限1</a></td><td>该参数表示基于覆盖的异频切换的A5事件的本服务小区RSRP门限1。如果服务小区RSRP测量值在异频A4A5时间迟滞InterFreqA4A5TimeToTrig内一直低于此门限，且邻区信号质量高于门限CovInterFreqA5SinrThld2，UE将上报A5事件。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A5 SINR触发门限2-12"><a href = " 
基于覆盖的异频A5 SINR触发门限2-12.html"> 
基于覆盖的异频A5 SINR触发门限2</a></td><td> 
该参数表示基于覆盖的异频切换的A5事件的邻区SINR门限2。如果服务小区RSRP测量值在异频A4A5时间迟滞InterFreqA4A5TimeToTrig内一直低于门限CovInterFreqA5SinrThld1，且邻区信号质量高于此门限，UE将上报A5事件。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A2 SINR触发门限-13"><a href = " 
基于覆盖的异频A2 SINR触发门限-13.html"> 
基于覆盖的异频A2 SINR触发门限</a></td><td>该参数表示基于覆盖的异频切换A2 SINR触发门限。如果服务小区SINR测量值在异频A1A2时间迟滞InterFreqA1A2TimeToTrig内一直低于该门限，将上报A2测量报告。参数的使用细节参见3GPP TS 38.331。</td></tr><tr><td id = " 
基于覆盖的异频A1 SINR触发门限-14"><a href = " 
基于覆盖的异频A1 SINR触发门限-14.html"> 
基于覆盖的异频A1 SINR触发门限</a></td><td> 
该参数表示基于覆盖的异频切换A1 SINR触发门限。如果服务小区RSRP测量值在异频A1A2时间迟滞InterFreqA1A2TimeToTrig内一直超过该门限，将上报A1测量报告。参数的使用细节参见3GPP TS 38.331。</td></tr></tbody></table>