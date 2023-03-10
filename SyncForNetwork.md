### 客户/服务器方式(C/S)和对等方式(P2P)

==客户/服务器(Client/Server,C/S)方式==

1. 客户和服务器是指通信中所涉及的两个应用进程。
2. 客户/服务器方式所描述的是进程之间服务和被服务的关系。
3. 客户是服务请求方，服务器是服务提供方。
4. 服务器总是处于运行状态，并等待客户的服务请求。服务器具有固定端口号（例如TTP服务器的默认端口号为80)，而运行服务器的主机也具有固定的IP地址。
5. C/S方式是因特网上传统的、同时也是最成熟的方式，很多我们熟悉的网络应用采用的都是C/S方式。包括万维网WWW、电子邮件、文件传输FTP等。
6. 基于C/S方式的应用服务通常是服务集中型的，即应用服务集中在网络中比客户计算机少得多的服务
   器计算机上。
7. 由于一台服务器计算机要为多个客户机提供服务，在C/S应用中，常会出现服务器计算机跟不上
   众多客户机请求的情况。为此，在C/S应用中，常用计算机群集（或服务器场）构建一个强大的虚拟服务器。

==对等(Peer-to-Peer,P2P)方式==

1. 在P2P方式中，没有固定的服务请求者和服务提供者，分布在网络边缘各端系统中的应用进程是对等
   的，被称为对等方。对等方相互之间直接通信，每个对等方既是服务的请求者，又是服务的提供者。
2. 目前，在因特网上流行的P2P应用主要包括P2P文件共享、即时通信、P2P流媒体、分布式存储等。
3. 基于P2P的应用是服务分散型的，因为服务不是集中在少数几个服务器计算机中，而是分散在大量对等计算机中，这些计算机并不为服务提供商所有，而是为个人控制的桌面计算机和笔记本电脑，它们通常位于住宅、校园和办公室中。
4. P2P方式的最突出特性之一就是它的可扩展性。因为系统每增加一个对等方，不仅增加的是服务的请求者，同时也增加了服务的提供者，系统性能不会因规模的增大而降低。
5. P2P方式具有成本上的优势，因为它通常不需要庞大的服务器设施和服务器带宽。为了降低成本，服务提供商对于将P2P方式用于应用的兴趣越来越大。

### 动态主机配置协议DHCP

动态主机配置协议DHCP(Dynamic Host Configuration Protocol)提供了一种机制，称为即插即用连网。这种
机制允许一台计算机加入新网络时可自动获取P地址等网络配置信息而不用手工参与。

DHCP主要使用以下报文来实现其功能：

1. DHCP DISCOVER:DHCP发现报文
2. DHCP OFFER:DHCP提供报文
3. DHCP REQUEST:DHCP请求报文
4. DHCP ACK:DHCP确认报文
5. DHCP NACK:DHCP否认报文
6. DHCP RELEASE:DHCP释放报文

DHCP报文在运输层使用UDP协议封装

DHCP客户使用的UDP端口号为68

DHCP服务器使用的UDP端口号为67

DHCP客户在未获取到IP地址时使用地址0.0.0.0

在每一个网络上都设置一个DHCP服务器会使DHCP服务器的数量太多。因此现在是使每一个网络至少有一个DHCP中继代理（通常是一台路由器），它配置了DHCP服务器的P地址信息，作为各网络计算机与DHCP服务器的桥梁。

![](https://fastly.jsdelivr.net/gh/1xingao/picgo@main/img/16728039421501672803941741.png)

### 电子邮件

![](https://fastly.jsdelivr.net/gh/1xingao/picgo@main/img/16729737435501672973743488.png)

### 万维网WWW

![](https://fastly.jsdelivr.net/gh/1xingao/picgo@main/img/16729759785221672975977921.png)

