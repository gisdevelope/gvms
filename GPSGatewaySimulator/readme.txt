
   GPSGatewaySimulator项目（GPS网关模拟器，以下简称GGS）用来为GPSTrackingMonitor系统（GPS跟踪系统，以下简称GTM）提供模拟的实时数据，他们之间通过UDP网络协议来进行通信。
   
   GGS提供的实时数据除了为GTM服务之外，还必须将其实时数据保存到数据库中，以便在GTM需要对特定车辆进行轨迹回放时为其提供车辆历史轨迹数据。
   
   因此，在GGS项目中，我们需要完成的功能包括：
   
   1、制定GGS、GTM和实时数据库之间的通信协议规范，这种规范要尽最大可能的满足三方通讯的便利性和高效性
   2、实时面向局域网广播车辆位置信息，并约定时间间隙
   3、实时数据库中轨迹数据的实时存储