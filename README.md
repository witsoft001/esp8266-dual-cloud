## ALINK + JOYLINK  

esp8288 支持双云对芯片（设备）支持同时控制与在线 APP 操控。  

> 有关 esp8266 对接 ALINK 的相关介绍请参考： [esp8266 + alink](https://github.com/espressif/esp8266-alink-v1.0)  
> 有关 esp8266 对接 JOYLINK 的相关介绍清参考：[esp8266 + joylink](https://github.com/espressif/esp8266-joylink)

### 1. 资源限制  

esp8266 在同时对接 alink + joylink 时，在正常工作和控制状态下，剩余内资源在 10k 左右，完全满足正常的控制需求。  

### 2. 使用

esp8266-double-cloud 在使用前，首先需要保证设备在 alink 的 阿里智能平台和 joylink 的京东微联平台分别注册成功，注册成功后运行本程序。  

首先进行 alink 配网和连接服务器，在连接成功后再发起设备对 joylink 对服务器的连接和数据获取。  

### 3. 注意事项  

在基于 esp8266 的使用中和其他云的组合应用中，需要准确处理上层应用的信号、时间、内存消耗等控制，以保证设备在双云模式下的正常运行。
