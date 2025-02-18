为解决工业领域数据接入上云过程中所面临的协议繁杂、设备异构化等问题，2020 年 9 月，[物联网边缘工业协议网关软件 Neuron](https://www.emqx.com/zh/products/neuron) 正式发布。

Neuron 提供了通过对各种工业协议转换实现的设备端数据采集、运行业务逻辑服务、警报判定，并将数据及警报上传及存储到云平台等功能，同时也可通过 Web 服务等部署和客户端应用软件，实现设备远程监控、远程维护、设备绩效管理、设备和资产管理等。

Neuron 工业网关南向支持接入主流的工业物联网协议（[驱动协议详细列表](https://static.emqx.net/resources/white-papers/neuron-driver-list-v1.4.pdf)）以及自定义协议的扩展。北向支持通过 [MQTT](https://www.emqx.com/zh/mqtt)、WebSocket 和 HTTP 协议与云平台层进行交互，实现设备上云与云端控制的能力。

**Neuron V1.2.0 现已正式发布**。

**下载地址：** [https://www.emqx.com/zh/downloads?product=neuron](https://www.emqx.com/zh/downloads?product=neuron)



## 新增 modbus: endianness 开关功能

我们在驱动配置时，有一个BYTEORDER（字节顺序）的选择，根据 little-endian 和 big-endian 两种排序方式，我们提供四种排序方式：

| BYTEORDER选择 | 排序方式 |
| :-----------: | :------: |
|       0       |  BE4321  |
|       1       |  BE3412  |
|       2       |  LE1234  |
|       3       |  LE2143  |


![WechatIMG21.png](https://static.emqx.net/images/81cd22f65da5d636e17d084c3e7085c1.png)


## 问题修复

- 修复 MQTT 获取趋势数据和获取日志问题；
- 修复 MQTT 发送信息失败而导致重连失败问题；
- 修复打开过多文件导致强制退出主进程问题；
- 修复在 32 位系统中，超出 2038 年时间戳数据溢出问题；
- 修复中文版 Linux 系统的本地语言的设置功能。



## 未来展望

作为新基建的重要组成部分，工业互联网已成为一个备受关注的热点领域。为了响应「中国制造 2025」及「工业 4.0」，越来越多的工业企业开始谋求数字化、智能化转型，工业设备上云也因此成为企业转型之路上必须面对的挑战。EMQ 于去年 10 月正式发布的云边一体化解决方案，可以实现异构设备连接及数据汇聚，完成后续边缘或云端计算，以云边协同的方式帮助领域内相关企业快速实现工业互联网架构下边缘层的功能。作为该方案重要组成部分的 Neuron，也将在未来持续为边缘工业互联网提供功能价值。

如果对 Neuron 有任何问题，请随时通过 [neuron@emqx.io](mailto:neuron@emqx.io) 联系我们。
