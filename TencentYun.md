# 2022年推荐算法效率开发必备工具榜单



## 一.引言

一个优秀的算法工程师应该至少具备3类能力：

基础能力：包含数理统计、机器学习、概率论以及深度学习等相关知识

编程能力：python、C++ or Java 以及基本的 Sql、linux、shell 命令

核心能力：对数据的敏感程度，对业务的理解程度以及 pipeline 的构建能力 

![img](https://pic1.zhimg.com/80/v2-d894a09795e8a9097586fd817fdbc2e6_1440w.jpg?source=d16d100b)




这些能力都需要我们不断地学习并实践开发，好的工具可以使我们专注于算法的研究与实现落地，下面整理了一份 2022 年推荐算法效率开发10大必备工具，榜单主要分以下3类，快来提高自己的开发效率吧！

![img](https://pic1.zhimg.com/80/v2-c5b92db93bf3bce605439fdf76034590_1440w.png?source=d16d100b)




**效率开发工具**：Pycharm、Idea、Iterm2

**辅助开发工具**：Grafana、Jprofile、Postman、Wakatime、Xxl-job

**云原生开发工具**：TKE、EMR

## 二.效率开发

鉴于目前算法工程师大都需要具备一定大数据开发的能力，所以 Python + Java / Scala 的开发趋势也逐渐兴起，python 负责 TF 相关算法的开发，Java / Scala 负责一些框架以及大数据处理的开发，下面介绍 3 款高效开发工具。

## 1.Pycharm

官网: https://www.jetbrains.com/pycharm/

![img](https://pic1.zhimg.com/80/v2-69994b3e5927762906655edcdaa8e0bc_1440w.png?source=d16d100b)



Pycharm 是一种 Python IDE（Integrated Development Environment，集成开发环境），带有一整套可以帮助用户在使用 Python 语言开发时提高效率的工具，例如调试、语法高亮、项目管理、代码跳转、智能提示、单元测试、版本控制以及依赖获取等。在原始功能基础上，其内部增加了丰富的插件。推荐算法工程师日常使用中最多的就是 Tensorflow、Keras、Pytorch、Sklearn、Numpy、Pandas 等，其中深度算法模型主要通过 Tensorflow 实现，由于 TF 不同版本的限制，用户使用 Pycharm 配合 Anonconda 可以轻松实现多 python 环境的构建，从而从容的切换多个 TF + PY 环境，实现多环境快速切换，效率开发。

智能补全示例：

![img](https://pic1.zhimg.com/80/v2-bc62a4389491328d3e1c39a9c4301d86_1440w.jpg?source=d16d100b)




## 2.Idea

官网: https://www.jetbrains.com/idea/

![img](https://picx1.zhimg.com/80/v2-1567c26cd1956b8e8a00c2a885253e45_1440w.jpg?source=d16d100b)




Idea 是 Java 语言开发的集成环境，是业界公认最好的 Java 开发工具之一，其具备便捷的代码提示、代码重构、智能补全功能，除此之外与各类版本工具例如 git、svn、github 都实现了完美整合，配合可定义的创新 GUI 设计，是Java / Scala 高效开发的不二之选。随着大数据的兴起，算法工程师的很多离线任务例如数据准备、特征处理、日志分析都离不开 Spark，而线上的实时任务例如实时请求、实时推荐则离不开 Streaming、Flink，通过离线 Spark + 在线 Flink 的模式构造 pipeline 管道，Idea 无疑是开发 Java / Scala 的利器，配合多款辅助插件，可以使开发更加得心应手。

智能联想示例：

![img](https://pica.zhimg.com/80/v2-e1dddf9d3bf40159e8052a129541c33b_1440w.jpg?source=d16d100b)




## 3.iterm2

官网：https://iterm2.com/

![img](https://pic1.zhimg.com/80/v2-61b74ce50069765a2276eff5dadf8d90_1440w.jpg?source=d16d100b)




作为代码与服务器沟通的桥梁，iterm2 是一款功能强大的终端工具，它支持分窗操作、自动补齐、粘贴历史、回放功能等，同时支持快捷键操作与自定义 UI，既美观又高效，正如官网说说，iterm2是 Terminal 的替代品，通过配置多个 Profiles 的 Advanced 选项，iterm2 可以实现多种自动化操作并支持多款插件，可以协助开发者更方便的进入终端并与集群完成交互。 

分屏监控示例：

通过快捷分屏可以同时实现 GPU 与 Top 指令，监测不同指标，也可以分屏处理终端的不同事务

![img](https://picx1.zhimg.com/80/v2-a87df9066428f79f1525d2bd86d9ed5e_1440w.png?source=d16d100b)




当然也可以换上自己最喜欢的背景，开发的感觉顿时焕然一新： 

![img](https://pic1.zhimg.com/80/v2-d0d5444585a1c74641ae57b7698a3bd4_1440w.png?source=d16d100b)




## 三.辅助开发工具

推荐算法工程师日常开发中离不开数据指标的监控、任务的部署、代码的优化、部门的协作以及工作总结，下面将基于以上几点为大家介绍经过实战考验的辅助开发工具。

## 1.Grafana

官网：https://grafana.com/grafana

![img](https://picx1.zhimg.com/80/v2-1d3af9f03108d2cb21f2f69f4f311b48_1440w.jpg?source=d16d100b)




随着业务的不断深化与发展，业务的种类增多、服务器数量加倍、数据网络压力增加的问题也接踵而至，这些问题都不可避免的带来线上事故的增多，因此随着业务体量逐渐扩大，相对应的服务器、应用状态、数据指标都应全方位监控，并且做到指标异常提前预警，Grafana 的出现完美解决了该问题。推荐算法场景下，从用户数据触发，到模型的训练上线，再到最终模型推理得到推荐结果，这一链路都存在诸多需要监控的指标，最基本的数据库以及数据集群、例如 Mysql、Redis、Hbase 以及 Kafka 等都需要做到时序的实时监控并做到异常报警，通过辅助组件状态的可视化提高线上作业的运维效率，有效减少故障发生后的响应时间。为此 Grafana 提供了快速灵活的可视化效果，可以让数据以任何想要的形式来可视化数据，例如时间序列、表、柱状图等等。

Redis 流量监控示例：

![img](https://pica.zhimg.com/80/v2-5ea085d4b020c9c12ee5b156017cd267_1440w.jpg?source=d16d100b)




Zookeeper 流量监控示例： 

![img](https://picx1.zhimg.com/80/v2-051ebb1c1efd8d94ebbae85495f4f501_1440w.png?source=d16d100b)




推荐场景下，由于与数据库交互较多，因此经常以时序的形式监控数据的读写状态，除此之外还有很多的形式提供，开发者可根据自己的需求灵活使用：

![img](https://picx1.zhimg.com/80/v2-5dcee5aee557c9f2fdaffe94194fb1ed_1440w.png?source=d16d100b)




## 2.Jprofile

官网：https://www.ej-technologies.com/products/jprofiler/overview.html

![img](https://pic1.zhimg.com/80/v2-ba493e288d07c861ff5bf681ee1ecbed_1440w.jpg?source=d16d100b)




JProfile 是一个重量级的 JVM 监控工具，提供对 JVM 的精确监控，其中堆遍历、CPU 剖析、线程剖析可视为定位当前系统瓶颈的得力工具，通过 JProfile 可以轻松定位 JVM 堆中的对象，优化内存并定位性能问题。除了可执行软件外，Jprofile 还支持 Idea 内置插件，轻松与开发环境的任务相匹配并分析，提高 JVM 代码分析能力，加速代码优化。推荐算法场景下，常见的就是召回、排序代码的构建，其中涉及很多需要优化的指标，例如与内存相关的物料库、与网络请求相关的 hbase访问速率等等，其都可以使用 JProfile 进行相关的分析，通过分析获取代码运行期间的瓶颈并作出响应优化，使得代码的编写更加合理高效。

相关指标的分析：

通过启动 JVM 进程与 JProfile 可以实时监测任务运行期间 JVM Memory、GC Activity、Classes 数量、Thread 数量、CPU Locd 参数

![img](https://picx1.zhimg.com/80/v2-16c74586cc04193ef0c42abb389b9bfd_1440w.png?source=d16d100b)




同时通过 Heap 分析可以分析 JVM 下各类数据占比，任务结束后可以通过 Snap 快照的形式获取当前任务内存占用较大的 Class，从而对症下药，定点优化，提升 JVM 程序效率。  

![img](https://picx1.zhimg.com/80/v2-d3a425726e93143584a3bc849ef91421_1440w.png?source=d16d100b)




## 3.Postman

官网：[Postman](https://www.postman.com/)

![img](https://picx1.zhimg.com/80/v2-c08b5186717ebcac18dea79bafc4f303_1440w.png?source=d16d100b)




Postman 是一款强大的网页调试工具的客户端，postman 为用户提供强大的 Web API & HTTP 请求调试功能。postman 能够发送任何类型的 HTTP 请求 (Get, Post, Put, Patch, Delete ...)，附带任何数量的参数+ headers，是一款非常实用的调试工具。推荐算法场景下，经常需要与其他团队进行交互协作，除了采用数据库交互外，常常使用 Http 接口的形式，返回一些代码所需的基础数据信息或者上下文信息。Postman 支持 多种 http 请求类型，支持在线存储数据，方便设置请求和 header 并支持不同的认证机制，同时提供响应数据自动高亮并在页面清晰展示，通过 postman 可以在开发前快速便捷的测试 http 请求的访问速度，访问结果等，而后快速应用到于实战代码中，非常的方便。

Http Get 请求：

下面给出了 postman 测试 get 请求的案例，开发者需指定 http 需求，并填写对应的 Headers 与 Query 请求参数，最后的结果可以选择通过 Json、Xml、Html 以及 Text 多种形式，同时 Http 响应时间也会在界面展示，便于开发者评估请求耗时。

![img](https://pic1.zhimg.com/80/v2-7c16feef4ef4782ec5fbaf7f35bb871f_1440w.jpg?source=d16d100b)




## 4.WakaTime

官网：https://wakatime.com/dashboard

![img](https://picx1.zhimg.com/80/v2-24a7be44f32f0c20175dda686884ca01_1440w.png?source=d16d100b)




WakaTime 是一款轻量级工作统计软件，其通过插件配置的方式内嵌到开发常用的办公开发软件中，在无感知的情况下统计相关工作时间，推荐算法场景下，常用的 Pycharm、Idea、CLion、VS Code、Word、Excel、PowePoint、iterm2、Sublime Text 等均适配 WakaTime。每天各个项目的开发时长、每天浏览网页与编码时间的对比、每日代码语言使用情况都可以详细记录其中。

![img](https://pica.zhimg.com/80/v2-8c4aa26cdb028bd9c5624572d86b8d94_1440w.png?source=d16d100b)




可以看到上面介绍的多款工具都可以用 WakaTime 进行时间统计，配合上 Git 的提交记录，顿时感觉自己的工作量满满，实战开发中可以根据 WakaTime 分析自己在各个项目的耗时情况，合理统筹分配时间。

![img](https://picx1.zhimg.com/80/v2-9d4874671593fb7502fa1895f08f06d6_1440w.png?source=d16d100b)




## 5.xxl-job 

官网：https://github.com/xuxueli/xxl-job/

![img](https://pica.zhimg.com/80/v2-1406279906bf1efa027d88e3861a582a_1440w.png?source=d16d100b)



xxl-job 是一个分布式任务调度平台，其核心设计目标是开发迅速、学习简单、轻量级与易扩展。现已开放源码，实现了开箱即用。其支持通过 Web 页面对任务进行 CRUD 操作，操作简单，支持动态修改任务状态，启动/停止任务以及终止运行中任务，即时生效。其可以看做是在 crontab 基础上的新型任务调度平台。推荐算法场景下，开发者经常需要打通 "数据-模型-上线-迭代-再上线" 的流程，而传统 crontab 定时控制局限性高，不支持跨集群部署任务，且在 shell 中部署串行任务每个子任务不易控制。为此 xxjob 解决了分布式环境下多机定时任务的调度问题，并提供了丰富的路由策略与完善的调度过期策略，支持动态分配与任务状态监控，适合推荐算法工程师部署数据分析、数据处理、模型训练、模型上线、模型 retrain 的定时任务链路。

**新增任务：**

每个任务都有一个单独的任务 ID，可以通过子任务 ID 连接父任务与子任务，达到跨集群调度的效果，同时支持堵塞处理策略，可以在一定程度上防止父任务执行失败，依旧执行错误子任务的情况。

![img](https://pica.zhimg.com/80/v2-fa46b473b28a3bf1bc0a9a2701ad7853_1440w.jpg?source=d16d100b)




###  四.云原生开发工具

云计算的概念从 2006 年提出距今已过 15 年，以宏观时间观看全社会对云计算的认知过程，基本经历了 "概念模糊 - IT 从业者认知 - IT 从业职推进 - 行业大众认知" 的四个过程，尤其 COVID-19 的出现，更是让大家体验到云会议、云办公、云协同、云课堂等云场景，加深了大家对云计算的认知。随着云计算的普及，推荐系统也由传统的老式集群模式逐渐向云计算迁移，在云计算时代，集群的变迁并不是简单的机房迁移，而是需要从思想到技术落地的全面改变。最理想的状态是数据存储、模型开发、单元测试、推荐系统部署等都在云上实现，正是基于这样的需求，促使了云原生技术的出现，同时基于当前推荐系统的演进与挑战，计算云原生、数据云原生、计算云原生也在行业内得到蓬勃发展。

## 1.TKE - Tencent Kubernetes Engine

### 1.1 TKE 简介

官网：https://cloud.tencent.com/product/tke

![img](https://pica.zhimg.com/80/v2-30c036224e970c0ba161ea5a80e3826d_1440w.jpg?source=d16d100b)



容器服务 TKE 是腾讯基于原生 Kubernetes 提供的高度可扩展的高性能容器管理服务。支持智能调度，获得国家级科技卓越奖，针对不同层级运维诉求和资源可控诉求，推出原生节点与超级节点适配不同企业需求，同时基于业务特点针对节点进行个性化优化，形态灵活，功能完备，兼容原生 Kubernetes API，助理企业降本增效。

![img](https://picx1.zhimg.com/80/v2-af5b2ed883c57d34b2ac8f08cf6fa5ac_1440w.png?source=d16d100b)




可以看到推荐系统在线、离线任务混杂、链路复杂，除此之外，还有各类数据仓库、网络接口、消息系统都内嵌到推荐系统中，使得推荐系统整体复杂度较高。其次面对日益增长的用户群体、商品库的不断丰富扩充，推荐系统面对的流量也日益增长，从而维持推荐系统的高并发与高可用对部署集群提出很高的要求。传统集群运行不稳定、运维不及时、无法适时扩容，影响推荐系统在线整体稳定性，除此之外由于资源利用的不合理也会大大增加企业成本，而腾讯云 TKE 则完美解决上述场景问题。

### 1.2 TKE x 小红书推荐系统实践

![img](https://pica.zhimg.com/80/v2-bae94cafa70a81385ffb26a327acafcd_1440w.png?source=d16d100b)



小红书的高速发展，得益于社区内容与兴趣用户之间的精准高效匹配，小红书推荐系统会根据用户的实时点击、推荐、收藏、评论等行为数据，实时更新用户画像，实时产生训练样本，实时训练模型，小时级迭代线上模型。

正如我们前面所说，复杂的推荐系统需要强大的底层服务，在稳定性的基础上，还需满足低延时与弹性扩容，腾讯 TKE 结合小红书场景特点，与小红书一起进行容器化改造，解决推荐系统场景下容器主要面对高并发对容器网络吞吐、稳定性与集群统一管理两大风险，实现了模型的小时级快速迭代， 大大提升了小红书笔记展示给用户的精准性与时效性。 在训练场景，借助容器服务的弹性能力，小红书也大幅降低了资源成本，节约成本达到 40% 以上。日常只需要 2 个 AI 工程人员负责训练平台底层资源运维的相关事项，团队可以把更多的精力和人力资源聚焦在算法优化上，不断提升模型的预测准确性。

## 2. EMR - 腾讯弹性 MapReduce

### 2.1.EMR 简介

官网：https://cloud.tencent.com/product/emr

![img](https://pic1.zhimg.com/80/v2-175a0ce88b6c6b58652d60f8ef9fb65c_1440w.jpg?source=d16d100b)




腾讯弹性 MapReduce 提供了高性能、高稳定性、按需灵活搭配的 Hive、Spark、Presto、Hbase、Flink、IceBerg、Alluxio 等丰富开源大数据组件，腾讯基于开源组件深度优化器性能与功能，使得 EMR 具备以下特性：

\- 丰富的一体化指标，支持用户自定义配置告警

\- 支持重要事件及作业现场的故障快速回朔，大幅提升运维效率

\- 按时间或按需自动负载、平滑扩缩集群资源、分钟级扩充海量算力，做到集群的缩放自如

\- 基于 VPC 网络隔离与安全组件保证网络安全可信

基于以上特性，腾讯 EMR 做到了资源的按需使用，在降低企业闲置成本的基础上，做到了集群的易于维护，完美适配推荐系统场景下的大数据任务需求。

![img](https://pica.zhimg.com/80/v2-f728f6bce5473a2948afe66fa926ccd5_1440w.png?source=d16d100b)




### 2.2 EMR x 知乎大数据集群升级实践

知乎是中文互联网最大的知识分享平台，数亿用户通过知识建立连接，找到感兴趣的高质量内容。为了将全平台的优质内容与终端用户更智能更高效的结合在一起，知乎对大数据平台对数据工具提出更实用要求，由于原集群存在资源交付率低，运维成本高等问题，知乎选择基于开源 Hadoop 技术栈构建的数千台规模的大数据集群无缝升级到腾讯云大数据云原生方案，该场景面临如下挑战：

**A.业务迁移 - 无感知**

为了保证改动对原先业务完全透明，需要在业务无感知情况下，对原大数据集群进行托管。为了实现该诉求，腾讯云采用定制化开放方案，构建基于知乎软件版本的镜像版本并产品化上线。由于在线资源 TKE 集群与离线 Hadoop 集群一般情况下均为错峰计算，为了解决原有资源的整体资源利用率，采用 EMR on TKE 方案，离线在线混合部署模式，提升整体资源利用率。在大数据 EMR 与 TKE 的融合过程中，为了保证离线任务与在线任务的隔离线，采用 Cgroup、BT 调度算法等方式做好资源隔离，防止离线任务资源侵占在线任务资源，影响线上服务的稳定性。例如训练任务启动过多节点侵占集群资源，导致线上推理任务存在资源、网络、IO 等风险。

![img](https://pic1.zhimg.com/80/v2-55fef7727646af6dc5a3d0f05162dccd_1440w.png?source=d16d100b)




**B.技术需求 - 版本兼容**

由于知乎原本的集群是基于开源 Hadoop 构建，这与腾讯云大数据版本之间存在差异， 因此需要提供一个可行的产品化方案来解决该问题 

除此之外，为了保证大数据 EMR 集群中任务运行的稳定性，腾讯云也对 Yarn 资源调度进行改造升级，保证资源调度时 AM 管理节点分配的合理性，同时也能做到资源弹性扩容到队列维度。

![img](https://picx1.zhimg.com/80/v2-f22f88485556ce4a0b38d6523ef9adae_1440w.png?source=d16d100b)



### 2.3 实践价值

基于腾讯云原生 TKE 方案，腾讯云团队探索出了 EMR 离在线混合部署策略，协助知乎由开源 Hadoop 集群无感知迁移至腾讯云大数据云原生方案，帮助知乎极大提升了资源利用率，从而大幅降低了技术成本，低峰期资源利用率提升高达5倍，达到了真正的降本增效。结合小红书与知乎的案例可以看到大数据下的推荐系统实战离、在线任务混合，对资源高效利用要求高，非常适配 EMR x TKE 的云原生解决方案。

## 五.总结

好的工具已经备好，希望各位优秀的程序员能够在各个工作利器的加持下，码到成功，码出精彩。更多好用工具可以扫码查看！！👇👇👇

![img](https://picx1.zhimg.com/80/v2-f46fb47ad0ac8618cf18a80078616786_1440w.png?source=d16d100b)



