![logo.png](https://github.com/SPLUG-GIT/yesterdayKite/blob/master/files/logo.png?raw=true)

__Visit  [our official web site](http://naver.github.io/pinpoint/)  for more information and  [Latest updates on Pinpoint](https://naver.github.io/pinpoint/news.html).__

## Latest Release (2020/09/09)
We're happy to announce the release of Pinpoint v2.1.0. Please check the release note at ([https://github.com/naver/pinpoint/releases/tag/v2.1.0](https://github.com/naver/pinpoint/releases/tag/v2.1.0)).

The current stable version is  [v2.1.0](https://github.com/naver/pinpoint/releases/tag/v2.1.0).

## Live Demo
Take a quick look at Pinpoint with our [demo](http://125.209.240.10:10123/main/ApiGateway@SPRING_BOOT/5m?inbound=1&outbound=4&wasOnly=false&bidirectional=false)!

## About Pinpoint
__Pinpoint**  is an APM (Application Performance Management) tool for large-scale distributed systems written in Java /  [PHP](https://github.com/naver/pinpoint-c-agent)/PYTHON. Inspired by  [Dapper](http://research.google.com/pubs/pub36356.html "Google Dapper"), Pinpoint provides a solution to help analyze the overall structure of the system and how components within them are interconnected by tracing transactions across distributed applications.

You should definitely check  **Pinpoint**  out If you want to

-  understand your [_application topology_]() at a glance
-   monitor your application in  _Real-Time_
-   gain  _code-level visibility_  to every transaction
-   install APM Agents  _without changing a single line of code_
-   have minimal impact on the performance (approximately 3% increase in resource usage)


## Getting Started
-   [Quick-start guide](https://naver.github.io/pinpoint/quickstart.html)  for simple test run of Pinpoint
-   [Installation guide](https://naver.github.io/pinpoint/installation.html)  for further instructions.

## Overview
Services nowadays often consist of many different components, communicating amongst themselves as well as making API calls to external services. How each and every transaction gets executed is often left as a blackbox. Pinpoint traces transaction flows between these components and provides a clear view to identify problem areas and potential bottlenecks.
For a more intimate guide, please check out our [_Introduction to Pinpoint_]() video clip.

* __ServerMap__ - Understand the topology of any distributed systems by visualizing how their components are interconnected. Clicking on a node reveals details about the component, such as its current status, and transaction count.
* __Realtime Active Thread Chart__   - Monitor active threads inside applications in real-time.

	-   **Request/Response Scatter Chart**  - Visualize request count and response patterns over time to identify potential problems. Transactions can be selected for additional detail by  **dragging over the chart**.
	![ss_call-stack.png](https://github.com/SPLUG-GIT/yesterdayKite/blob/master/files/ss_call-stack.png?raw=true)


	**CallStack** - Gain code-level visibility to every transaction in a distributed environment, identifying bottlenecks and points of failure in a single view.
	(![ss_inspector.png](https://github.com/SPLUG-GIT/yesterdayKite/blob/master/files/ss_inspector.png?raw=true) )

	**Inspector**  - View additional details on the application such as CPU usage, Memory/Garbage Collection, TPS, and JVM arguments.

	[![Inspector](https://github.com/naver/pinpoint/raw/master/doc/images/ss_inspector.png)](https://github.com/naver/pinpoint/blob/master/doc/images/ss_inspector.png)


	## Supported Modules
	-   JDK 6+
	-   [Tomcat 6/7/8/9](https://github.com/naver/pinpoint/tree/master/plugins/tomcat),  [Jetty 8/9](https://github.com/naver/pinpoint/tree/master/plugins/jetty),  [JBoss EAP 6/7](https://github.com/naver/pinpoint/tree/master/plugins/jboss),  [Resin 4](https://github.com/naver/pinpoint/tree/master/plugins/resin),  [Websphere 6/7/8](https://github.com/naver/pinpoint/tree/master/plugins/websphere),  [Vertx 3.3/3.4/3.5](https://github.com/naver/pinpoint/tree/master/plugins/vertx),  [Weblogic 10/11g/12c](https://github.com/naver/pinpoint/tree/master/plugins/weblogic),  [Undertow](https://github.com/naver/pinpoint/tree/master/plugins/undertow)
	-   Spring, Spring Boot (Embedded Tomcat, Jetty, Undertow), Spring asynchronous communication
	-   Apache HTTP Client 3.x/4.x, JDK HttpConnector, GoogleHttpClient, OkHttpClient, NingAsyncHttpClient, Akka-http, Apache CXF
	-   Thrift Client, Thrift Service, DUBBO PROVIDER, DUBBO CONSUMER, GRPC
	-   ActiveMQ, RabbitMQ, Kafka
	-   MySQL, Oracle, MSSQL(jtds), CUBRID, POSTGRESQL, MARIA
	-   Arcus, Memcached, Redis([Jedis](https://github.com/naver/pinpoint/blob/master/plugins/redis),  [Lettuce](https://github.com/naver/pinpoint/tree/master/plugins/redis-lettuce)), CASSANDRA, MongoDB, Hbase, Elasticsearch
	-   iBATIS, MyBatis
	-   DBCP, DBCP2, HIKARICP, DRUID
	-   gson, Jackson, Json Lib, Fastjson
	-   log4j, Logback, log4j2

	## Compatibility
	Java version required to run Pinpoint:

	|Pinpoint Version|Agent|Collector|Web|
	|-----------|---|---|---|
	|1.5.x|6-8|7-8|7-8|

	HBase compatibility table:

	|Pinpoint Version|HBase 1.0.x|HBase 1.2.x|HBase 1.4.x|HBase 2.0.x|
	|-------------|---|---|---|---|
	|1.5.x|yes|not tested|not tested|no|

	Agent - Collector compatibility table:

	|Agent Version|Collector 1.5.x|Collector 1.6.x|Collector 1.7.x|Collector 1.8.x|Collector 2.0.x|Collector 2.1.x|
	|--------------|---|---|---|---|---|---|
	|1.5.x|yes|yes|yes|yes|yes|

	Flink compatibility table:

	|Pinpoint Version|flink 1.3.X

	flink 1.4.X|flink 1.5.X|flink 1.6.X|flink 1.7.X|1.7.x|
	|--------|---|---|---|---|
	|yes|yes|no|no|no|

	## Community
	[Github issues]()
	[Google group]()
	[Gitter]()
	We have Chinese community now, welcome to join!

	|QQ Group1: 897594820|QQ Group2: 812507584|DING Group|
	|----|----|----|
	| | | |

	## License
	Pinpoint is licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/naver/pinpoint/blob/master/LICENSE) for full license text.

	```
	Copyright 2018 NAVER Corp.

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

	    http://www.apache.org/licenses/LICENSE-2.0

		Unless required by applicable law or agreed to in writing, software
		distributed under the License is distributed on an "AS IS" BASIS,
		WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
		See the License for the specific language governing permissions and
		limitations under the License.
		```

