# 快速部署 Flowise 社区版

## 概述


FlowiseAI 是一个开源的低代码开发工具，专为开发者构建定制的语言学习模型（LLM）应用而设计。 通过其拖放式界面，用户可以轻松创建和管理AI驱动的交互式应用，如聊天机器人和数据分析工具。 它基于LangChain框架，支持与多种AI模型和数据库集成，实现高度可定制化的流程自动化​。 详情请看[Flowise官网](https://docs.flowiseai.com/)。

## 计费说明

Flowise在计算巢上的费用主要涉及：

- 所选vCPU与内存规格
- 磁盘容量
- 公网带宽

计费方式：按量付费（小时）

预估费用在创建实例时可实时看到。

## 部署架构

Flowise社区版是单机部署架构。

## RAM账号所需权限

Flowise服务需要对ECS、VPC等资源进行访问和创建操作，若您使用RAM用户创建服务实例，需要在创建服务实例前，对使用的RAM用户的账号添加相应资源的权限。添加RAM权限的详细操作，请参见[为RAM用户授权](https://help.aliyun.com/document_detail/121945.html)
。所需权限如下表所示。

| 权限策略名称                          | 备注                         |
|---------------------------------|----------------------------|
| AliyunECSFullAccess             | 管理云服务器服务（ECS）的权限           |
| AliyunVPCFullAccess             | 管理专有网络（VPC）的权限             |
| AliyunROSFullAccess             | 管理资源编排服务（ROS）的权限           |
| AliyunComputeNestUserFullAccess | 管理计算巢服务（ComputeNest）的用户侧权限 |
| AliyunCloudMonitorFullAccess    | 管理云监控（CloudMonitor）的权限     |


## 部署流程

1. 单击[部署链接](https://computenest.console.aliyun.com/service/instance/create/cn-hangzhou?type=user&ServiceId=service-f462f9b21cb7477381f0)，进入服务实例部署界面。
2. 选择新建ECS实例并根据界面提示配置参数，配置完成后点击下一步：确认订单。

    <img src="1.jpg" width="1400" align="bottom"/>
   
3. 点击立即创建，等待服务实例创建完成。

   <img src="2.jpg" width="1400" align="bottom"/>

4. 服务实例创建成功后，进入服务实例详情页。在概览页可获取Flowise登录信息。
   
   <img src="3.jpg" width="1400" align="bottom"/>

5. 点击外网面板地址访问Flowise服务。
   
   <img src="4.jpg" width="1400" align="bottom"/>