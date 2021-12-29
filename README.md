# EasyModbus
最简单好用的Modbus控件
根据EasyModbus修改而来，修复了几个bug，增加了几个接口，简单好用。
.NET版本Modbus TCP、Modbus UDP、Modbus RTU client/server库

支持的功能代码：
读线圈(FC1)
读取离散输入(FC2)
读寄存器(FC3)
读输入寄存器(FC4)
写单线圈(FC5)
写入单个寄存器(FC6)
写多个线圈(FC15)
写入多个寄存器(FC16)
读/写多个寄存器(FC23)

***************************************************************************************
ModbusServer修改版：
***************************************************************************************
2020-8-13：解决ModbusUDP无法二次启动问题 关闭未结束线程 listenerThread
2020-8-2：增加ReceiveDataChanged(Byte[] data) SendDataChanged(Byte[] data)回调
2020-8-2：解决从机模式接收数据debug信息全部为00的问题
2020-8-1：增加ModbusType 规范化编程
2020-8-1：解决UDP从机模式关闭后不能打开的问题
2020-7-30：解决ModbusRTU从机模式下数据接收错误的问题 详见:SerialHandler

***************************************************************************************
ModbusClient修改版：
***************************************************************************************
2020-8-15：增加响应延时属性ResposeDelay 事件ResposeDelayChanged
2020-8-11：修正Modbus主机模式下退出报不能为Null异常错误 详见:~ModbusClient()
2020-8-11：修正UDP连接connected属性一直为True的问题
2020-8-2：规范化ReceiveDataChanged(Byte[] data) SendDataChanged(Byte[] data)回调
2020-8-1：增加ModbusType 规范化编程
2020-8-1：增加UDP模式发送回传（全模式支持发送、接收通信数据回传）
2020-7-31：修正Modbus主机模式下连接超时 详见:connectTimeout 
***************************************************************************************

EasyModbus development team:
I don't know how to use the GitHub website. I am very optimistic about the easymodbus control.
If the easymodbus developer notices this code, please contact me and I want to join.

李锦上lijinshang@126.com
