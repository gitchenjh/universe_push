# 推送sdk nio版本
客户端sdk需要长连接服务建立链接，需要注意以下问题
* push-connector多机房部署，需要选取最合适的ip地址链接
* 消息可靠性了解，如果需要需要确认推送是否完整到达用户，可以自定义ack机制
* 多种链接支持，http，tcp，udp，在手机电量允许情况下，允许用户主动发起请求重新建立链接，从而获取离线消息