# 四象SCADA系统_SxScada

#### 介绍
四象SCADA系统是一款通用性硬件网关控制系统，可应用于智慧城市、交通、消防、电力、能源、水务、水利、环保、气象、军事等工控物联网数据采集的通用性硬件采集/控制系统。

四象SCADA系统部署在pc电脑、云服务器中，就变成了一个软网关;

四象SCADA系统部署在arm工控板(例如：rk3288、rk3566、rk33399、rk3588)中，就变成了一个功能强大的工业边缘计算网关。

无需用户专业编程，简单在web后台管理系统中设置几步后，即可将复杂多变的各类工控硬件动态接入到四象SCADA系统中，数据中心计算模块会将设备的实时数据进行动态转换并动态以多协议方式输出，将协议还原成真实设备数据（状态、属性），预警功能还可以根据设备的属性实时进行实时报警或者联动控制。
同时，四象SCADA系统还自带数据中心大屏设计、单机组态功能，可以任意实现需要显示的大数据大屏展示，可为APP/WEB提供强大的数据支撑。
四象SCADA系统能完全替代plc，实现数据控制功能，性能是plc处理数据的1000倍以上。

**数据输入：**
支持同时输入各类dtu、modbus-rtu、modbus-tcp、opc-ua、mqtt、各类原生plc协议、可动态集成各厂家的web接口.

**数据输出：**
支持同时输出modbus-tcp、opc-ua、web接口、web接口、写入数据库（mysql/mssql/oracle/sybase/progresql/redis/mongo)、写入中间件(kafka,mqtt)、写入索引库(elasticsearch、solr)等.

**负载并发：**可以每秒管理1-1000万个数据设备的状态和实时数据获取。

**使用：**
无需编程，在后台管理后台配置接入网关和硬件规则即可。

**核心特性**
多通道设备接入,无限设备管理
1.可以直接同时接入各类dtu、modbus-rtu、modbus-tcp、opc-ua、opc-da、mqtt、各类原生plc协议、可动态集成各厂家的web接口,直接同步接入设备的硬件数据，动态还原出设备属性及实时数据;
2.可以通过tcp/udp/mqtt/,tls/dtls等方式接入任意报文，通过消息总线方式进入统一集中管理数据数据

强大的规则引擎
强大的可视化规则编辑功能，根据设置的规则触发相应条件，产生实时设备告警及场景联动控制.

**技术栈**
web管理系统：java，html+js+css
数据采集端：java

联系Q:3328350766

#### 软件更新
版本：1.0.0	完成时间：2021-09-05

内容：完成scada系统功能，包括产品中心、数据中心、数据分析、大屏设计、系统管理等功能

版本:	1.0.1	更新时间：2021-11-01

内容：修复modbus-rtu数据采集bug

版本： 1.0.2	更新时间：2021-11-05

内容：完善大屏管理功能

版本：2.0.1	更新时间：2022-06-1

将从串口采集线程、串口写入线程 采集消息队列化缓存处理，防止因同时读写同一串口造成系统崩溃； 优化modbus-rtu、modbus-tcp数据采集速度； 增加“云”同步功能，软件会将当前启动用的设备信息及实时数据上传到“四象物联云平台”私有化部署版中；会自动将云平台的“产品库”下载到本地中；会实时监听云平台的控制下发指令； 增加“云”控制功能，可以通过在本SCADA系统中执行任意SCADA中的设备的数据； 增加“启动控制”功能，可以实现开机实现自定义动作流程，支持APP实现某行业控制的“一键开机”功能； 增加“停止控制”功能，可以实现关机实现自定义动作流程，支持APP实现某行业控制的“一键关机”功能； 增加“变量管理”功能，可以实现两个设备的属性值逻辑运算结果； 增加“变量联动控制”功能，通过变量值实现自定义的条件联动功能，达到某行业的多点设备控制功能； 增加内置行业控制逻辑，能源节能控制行业的水泵、变频器、中央空调主机离心机动态控制功能，可以实现通过冷冻泵、冷却泵之间的温差来动态控制变频器的频率；

版本：3.0.1	更新时间：2023-3-1

增加各类dtu硬件接入，增加dtu-modbus-rtu、dtu-modbus-tcp、tcp/udp/websocket自定义解析功能，增加云平台下发到dtu、tcp自定义客户端的指令控制

版本：2024.0.1	更新时间：2024-1-1

增加组态管理，可以添加修改组态图，组态图中可以直接绑定设备的属性、需要执行的功能等。

版本：2024.0.3	更新时间：2024-3-1

增加实时数据曲线显示功能、增加用画笔修改历史数据功能、历史数据分列直观管理

增加产品属性修改显示的颜色

版本：2024.0.3	更新时间：2024-7-25
优化代码结构
增加网关与云平台的安全鉴全功能、优化修改云配置之后无需等待。

增加网关内部指令操作功能

#### 软件架构
四象工业网关业务架构图
![输入图片说明](https://www.sxlinks.com/static/scada/images/软件架构/四象工业网关业务架构图.png)
四象物联设备接线示意图
![输入图片说明](https://www.sxlinks.com/static/scada/images/软件架构/四象物联设备接线网络示意图.png)
四象工业网关系统架构图
![输入图片说明](https://www.sxlinks.com/static/scada/images/软件架构/软网关系统架构图.png)


#### 安装教程
登录
![输入图片说明](https://www.sxlinks.com/static/scada/images/登录.png)
首页
![输入图片说明](https://www.sxlinks.com/static/scada/images/首页.png)
首页-普通用户
![输入图片说明](https://www.sxlinks.com/static/scada/images/首页_普通用户.png)


产品中心-产品管理
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/产品管理/产品_列表.png)
产品中心-产品详情
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/产品管理/产品_编辑.png)
产品中心-产品属性列表
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/产品管理/产品_属性_列表.png)
产品中心-产品属性详情
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/产品管理/产品_属性_编辑.png)
产品中心-设备列表
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/设备管理/设备_列表.png)
产品中心-设备详情
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/设备管理/设备_编辑.png)
产品中心-设备属性列表
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/设备管理/设备_属性_列表.png)
产品中心-设备属性详情
![输入图片说明](https://www.sxlinks.com/static/scada/images/产品中心/设备管理/设备_属性_编辑.png)
规则管理-启动控制
![输入图片说明](https://www.sxlinks.com/static/scada/images/规则引擎/启动控制/启动控制列表.png)
![输入图片说明](https://www.sxlinks.com/static/scada/images/规则引擎/启动控制/启动控制编辑.png)
规则管理-停止控制
![输入图片说明](https://www.sxlinks.com/static/scada/images/规则引擎/停止控制/停止控制列表.png)
![输入图片说明](https://www.sxlinks.com/static/scada/images/规则引擎/停止控制/停止控制编辑.png)
规则管理-变量管理
![输入图片说明](https://www.sxlinks.com/static/scada/images/规则引擎/变量管理/变量管理列表.png)
![输入图片说明](https://www.sxlinks.com/static/scada/images/规则引擎/变量管理/变量管理编辑.png)
web接口
![输入图片说明](https://www.sxlinks.com/static/scada/images/web接口/接口列表.png)

#### 使用说明

1.  xxxx
2.  xxxx
3.  xxxx

#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request
