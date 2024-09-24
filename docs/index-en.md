<h1> Rapid Deployment Flowise Community Edition </h1>

<h2> Overview </h2>

<p>FlowiseAI is an open source low-code development tool designed for developers to build custom language learning model (LLM) applications. Through its drag-and-drop interface, users can easily create and manage AI-driven interactive applications such as chatbots and data analytics tools. It is based on a LangChain framework and supports integration with multiple AI models and databases for highly customizable process automation. For more information, see <a href = "https://docs.flowiseai.com/">Flowise website </a>. </p>

<h2> Billing instructions </h2>

<p> The cost of the Flowise in calculating the nest mainly involves:</p>

<ul>
<li> Selected vCPU and Memory Specifications </li>
<li> Disk capacity </li>
<li> Internet bandwidth </li>
</ul>

<p> Billing method: Pay-As-You-Go (hourly)</p>

<p> The estimated cost is visible in real time when the instance is created. </p>

<h2> Deployment Architecture </h2>

<p>Flowise Community Edition is a stand-alone deployment architecture. </p>

<h2> Permissions required for RAM accounts </h2>

<p>Flowise services need to access and create resources such as ECS and VPC. If you use a RAM user to create a service instance, you need to add the corresponding resource permissions to the account of the RAM user before creating the service instance. For more information about how to add RAM permissions, see <a href = "https://help.aliyun.com/document_detail/121945.html"> Authorize RAM users </a>.
. The required permissions are shown in the following table. </p>

<table>
<thead>
<tr>
<th> Permission policy name </th>
<th> Remarks </th>
</tr>
</thead>
<tbody>
<tr>
<td>AliyunECSFullAccess</td>
<td> Permissions to manage ECS </td>
</tr>
<tr>
<td>AliyunVPCFullAccess</td>
<td> Permissions for managing VPC networks </td>
</tr>
<tr>
<td>AliyunROSFullAccess</td>
<td> Manage permissions for Resource Orchestration Services (ROS) </td>
</tr>
<tr>
<td>AliyunComputeNestUserFullAccess</td>
<td> Manage user-side permissions for the compute nest service (ComputeNest) </td>
</tr>
<tr>
<td>AliyunCloudMonitorFullAccess</td>
<td> Permissions to manage CloudMonitor (CloudMonitor) </td>
</tr>
</tbody>
</table>

<h2> Deployment process </h2>

<ol>
<li> Click <a href = "https://computenest.console.aliyun.com/service/instance/create/cn-hangzhou?type=user&ServiceId=service-f462f9b21cb7477381f0"> Deployment Link </a> to go to the Service Instance Deployment page. </li>
<li><p> Select the new ECS instance and configure the parameters according to the interface prompts. After the configuration is complete, click Next: Confirm Order. </p>

<p><img src="1.jpg" width="1400" align="bottom"/></p></li>
<li><p> Click Create Now and wait for the service instance to be created. </p>

<p><img src="2.jpg" width="1400" align="bottom"/></p></li>
<li><p> After the service instance is successfully created, go to the service instance details page. The Flowise login information is available on the Overview page. </p>

<p><img src="3.jpg" width="1400" align="bottom"/></p></li>
<li><p> Click the external network panel address to access the Flowise service. </p>

<p><img src="4.jpg" width="1400" align="bottom"/></p></li>
</ol>
