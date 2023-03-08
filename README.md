# 手动构造TCP
本项目是基于CS144课程实现的，把可靠的字节流构造为TCP传输协议  
- 实现了支持读写的字节流模块。
- 实现流重组器，支持将乱序的子串按正确的顺序缝合回连续的字节流中。
- TCPReceiver端，利用流重组器将TCP包的内容组装进字节流中，同时实现流量控制
- TCPSender端，发送字节流，同时根据窗口信息调整窗口，能够进行超时重传。
- 管理TCPConnection，把上述的TCPReceiver和TCPSender实现连接。  
默认的branch master是lab0的解答，构造了基本的字节流  
lab1实现了TCP接收所需的流重组器  
lab2实现了TCP接收器  
lab3实现了TCP发送器  
lab4实现了TCP连接器  

### 所有实现均正确通过了check_lab
