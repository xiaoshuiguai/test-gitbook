## 安保适配器之间关系

1. 车队通过手机安装`App`，与`HiLEG_IST`适配器连接。
2. `HiLEG_IST`适配器向mq主题HIATMP.HISENSE.GPS发送报文。
3. `LEG_GPS_SERVER`接收**HIATMP.HISENSE.GPS**报文，处理后入数据库LEG_GPS_DATA表；同时向mq主题HIATMP.HISENSE.HILEG.GPSINF发送车队进行数据。
4. 信号自动勤务接受**HIATMP.HISENSE.HILEG.GPSINF**数据，进行信号灯控制。

  

![1](project.png)
