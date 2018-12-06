# searchAndRecommendEngine
搜索系统和 推荐系统技术资料整理
这篇博客意图是收集市面上质量不错的搜索引擎技术资料，内容来源包括开源项目官网（Lucene、Solr、Elastic）、综合技术网站（infoQ、Stackoverflow、github 等）、专业技术网站（我爱自然语言处理等）、国内外知名互联网公司技术博客（阿里中间件团队博客、美团技术博客等）、知名技术牛人博客（Matrix67、刘超觉先等）等。
以下整理的内容大致根据来源进行分类，等这篇整理得差不多了再开一篇博客根据知识点进行梳理。
个人视角有限，还望各位同行补充、丰富，谢谢。

* * *

## 开源相关

### Lucene

*   [Lucene 官网](https://lucene.apache.org/)

*   [Lucene Wiki](https://wiki.apache.org/lucene-java/FrontPage)

*   [索引结构 -Lucene6.6.0](https://lucene.apache.org/core/6_6_0/core/org/apache/lucene/codecs/lucene62/package-summary.html#package.description)

    ### Solr

*   [Solr 官网](http://lucene.apache.org/solr/)

*   [Solr Wiki](https://wiki.apache.org/solr/)

    ### Elastic

*   [Elastic 官网](https://www.elastic.co/cn/)

*   [Elastic Blog](https://www.elastic.co/blog#sthash.khjrgPU5.dpbs)

*   [Elastic Formus](https://discuss.elastic.co/)

*   [Elasticsearch: 权威指南 - 中文版](https://www.elastic.co/guide/cn/elasticsearch/guide/current/index.html)

*   [Elastic 中文社区](https://elasticsearch.cn/)

    ### LucidWorks

*   [LucidWorks](https://lucidworks.com/)

*   [LucidWorks Blog](https://lucidworks.com/blog/#blog/)

    ### 中文分词

*   [ansj 分词](https://github.com/NLPchina/ansj_seg?)

*   [HanLP 分词](https://github.com/hankcs/HanLP)

*   [ES-Analysis-IK](https://github.com/medcl/elasticsearch-analysis-ik)

## 大公司

### 阿里

*   [天猫推荐算法团队的那些事儿 - 20140401 - infoQ](https://www.infoq.cn/article/2014%2F04%2Ftmall-recommendation-team)
    _本文以访谈的方式呈现，对搜索和推荐算法进行了简单的比较，提到了 AB 测试和离线测试，主要对推荐算法团队的工作方式、工作考评、任务分配、招聘等进行了介绍。_

*    推荐：[天池大数据竞赛](https://hacpai.com/forward?goto=https%3A%2F%2Ftianchi.aliyun.com%2Fcompetition%2Findex.htm%3Fspm%3D5176.100065.111.2.EdzxZN%26id%3D) [天池数据集](https://hacpai.com/forward?goto=https%3A%2F%2Ftianchi.aliyun.com%2Fdatalab%2Findex.htm%3Fspm%3D5176.100066.1234.9.WioQNV)

*   [天猫 11.11：搜索引擎实时秒级更新 - 20141111 - infoQ](https://www.infoq.cn/article/2014%2F11%2Ftmall-1111-search-engine)
    _文章简单介绍了阿里搜索引擎架构，提到了以下内容：1）为提高数据实时性（库存、价格等），去掉应用层和业务层的缓存，重点提升引擎层的服务能力。2）排序链，根据业务场景定制排序链。3）sku 搜索，搜索结果和属性导航联动（标类产品）。_

*   [基于 Hadoop 生态技术构建阿里搜索离线系统（视频） - 20141205 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fpresentations%2Falibaba-search-offline-system-based-on-hadoop)
    _主要介绍了：1）阿里搜索业务（1688、淘宝、天猫、一淘、openSearch）；2）搜索技术体系；3）搜索离线系统；4）实时计算方案；5）集群优化与管理；_
*   [阿里搜索离线技术团队负责人谈 Hadoop：阿里离线平台、YARN 和 iStream](https://www.infoq.cn/article/2014%2F09%2Fhadoop-alibaba-yarn)

*   [基于 Apache Flink 的实时计算引擎 Blink 在阿里搜索中的应用 - 20170216 - infoQ](https://www.infoq.cn/article/real-time-computing-engine-blink-in-alibaba-search)

**阿里搜索事业部技术团队**
阿里集团搜索、推荐、图像技术的大本营，大数据时代的创新主场。

*   [阿里搜索事业部技术团队](https://yq.aliyun.com/teams/23?spm=5176.100239.0.0.IlfIYv)

*   [OpenSearch：轻松构建大数据搜索服务 - 20160222](https://yq.aliyun.com/articles/67156?spm=a2c4e.11163080.searchblog.9.56c42ec17lRdd2)

*   [搜索双链路实时计算体系 @双 11 实战 - 20160111](https://yq.aliyun.com/articles/2699?spm=5176.100244.teamhomeleft.95.WweKDa)

**阿里中间件团队博客**
2012 年期间，阿里中间件博客记录了 20 多篇 Lucene、Solr 相关博文，主要记录了一些在项目开发过程中遇到的问题，以及部分源码解读。内容丰富、实用，但不是很系统。

*   [阿里中间件团队博客](http://jm.taobao.org/)

*   [Solr 调优参考 - 20120521](http://jm.taobao.org/2012/05/21/solr-tuning)

*   [Solr Lucene 优劣势分析 - 20120626](http://jm.taobao.org/2012/06/26/solr-lucene-advantages-and-disadvantages)

*   [SolrQuery 性能压测参考 - 20120731](http://jm.taobao.org/2012/07/31/solr-query-performance-test-reference)

*   [NumericField NumericRangeQuery 原理分析 - 20120731](http://jm.taobao.org/2012/07/31/numeric-field-numeric-range-query)

*   [Solr schema 编写指导 - 20120731](http://jm.taobao.org/2012/07/31/solr-schema-guide)

*   [关于搜索挖掘所想 - 20120731](http://jm.taobao.org/2012/07/31/think-about-search/)

*   [SolrQuery 挖掘 -- 单维度聚合分析 - 20120920](http://jm.taobao.org/2012/09/20/solrquery-mining)

*   [我感受到的排序机制参考 - 20120920](http://jm.taobao.org/2012/09/20/sort-of-mechanism-reference)

*   [垂直搜索新问题 - 20120920](http://jm.taobao.org/2012/09/20/vertical-search-new-question)

*   [Solr 平台化搜索实战必知场景 - 20120921](http://jm.taobao.org/2012/09/21/solar-search)

*   [Solr Schema 配置小细节大问题 - 20121015](http://jm.taobao.org/2012/10/15/solr-schema-configuration-problem/)

*   [Solr DisjunctionMax 注解 - 20121015](http://jm.taobao.org/2012/10/15/solr-disjunctionmax/)

*   [Sql Support within Solr- 类 Sql 的 solr 搜索实现 (1) - 20121015](http://jm.taobao.org/2012/10/15/sql-support-within-solr)

*   [Sql Support within Solr- 类 Sql 的 solr 搜索实现 (2) - 20121015](http://jm.taobao.org/2012/10/15/solr-flux-source-code-sql-support-within-solr/)

*   [关于 TrieField 的全面认识、理解、运用 - 20121015](http://jm.taobao.org/2012/10/15/learn-about-triefield)

*   [Solr Facet 引发思考 on the road - 20121029](http://jm.taobao.org/2012/10/29/solr-facet-on-the-road/)

*   [查询问题 ---queryparse 深入理解 - 20121029](http://jm.taobao.org/2012/10/29/deep-learn-queryparse)

*   [TermRangeQuery 源码解析 - 20121106](http://jm.taobao.org/2012/11/06/termrangequery-source-code)

*   [Solr 之缓存篇 - 20121106](http://jm.taobao.org/2012/11/06/solar-cache/)

*   [搜索的测试话题 - 20121113](http://jm.taobao.org/2012/11/13/test-topic-about-search)

*   [关于搜索夜话 ---- 作为阶段序列的告别 - 20121113](http://jm.taobao.org/2012/11/13/night-talk-about-search/)

*   [solr 长文本搜索问题 - 20121210](http://jm.taobao.org/2012/12/10/solr-long-text-search-problem)

*   [SolrCore2.9.1 源码分析备忘 - 20121210](http://jm.taobao.org/2012/12/10/solr-core-2-9-1-source-code-analyse)

### 百度

*   [百度万亿量级数据库 Tera 架构应用、设计与实践全攻略 - 20170526 - infoQ](https://www.infoq.cn/article/2017%2F05%2Fdatabase-baidu-Tera)

### 京东

*   [京东 618：揭秘大促销背后的个性化推荐 - 20150618 - infoQ](https://www.infoq.cn/article/2015%2F06%2Fjd-618-personalrecommendation)

*   [京东 11.11：商品搜索系统架构设计 - 20151111 - infoQ](https://www.infoq.cn/article/jingdong-11-11-commodity-search-system-architecture-design?utm_source=6aiq.com)

*   [京东 618：机器学习与商品数据挖掘和知识抽取 - 20170618 - infoQ](https://www.infoq.cn/article/2017%2F06%2Fjd-618-Machine-learning-commodit)

### 美团点评

**美团点评技术团队博客**
在国内互联网公司中，个人认为“美团点评技术团队博客”是最持之以恒的，而且非常干货。

*   [美团点评技术团队](https://tech.meituan.com/)

*   [美团 O2O 排序解决方案——线下篇 - 20151207](https://tech.meituan.com/rerank_solution_offline.html)

*   [美团点评旅游搜索召回策略的演进 - 20170616](http://www.6aiq.com/article/1522247441467)

### 携程

*   [携程技术中心](https://cloud.tencent.com/developer/column/2048/tag-10149/page-8)

### 去哪儿

*   [去哪儿网机票搜索系统的高并发架构设计 20170421 - infoQ](http://www.6aiq.com/article/1522670952812)


### 搜狗

*   [搜狗搜索广告检索系统 - 弹性架构演进之路 - 20160111 - infoQ](https://mp.weixin.qq.com/s?__biz=MzI4MTY5NTk4Ng==&mid=2247489709&idx=1&sn=dd82cbae0f01a13fcef39ac2925c6406&chksm=eba41b30dcd3922697fcbdd22188d919803c40841609f4a1280355b251b68a4d786fddcc8fb6&scene=27#wechat_redirect)

*   [深度学习在搜狗无线搜索广告中的应用 - 20160808 - infoQ](https://www.infoq.cn/article/2016%2F08%2Fsougou-deep-learing-wireless-sea)

*   [以搜狗为例，谈语音输入如何影响你的生活 - 20161208 - infoQ](https://www.infoq.cn/article/2016%2F12%2Fsougou-Voice-input-life)
### 一号店

*   [1 号店 11.11：分布式搜索引擎的架构实践 - 20151112 - infoQ](https://www.infoq.cn/article/yhd-11-11-distributed-search-engine-architecture)

*   [1 号店 11.11：机器排序学习在电商搜索中的实战 - 20161111 - infoQ](http://www.6aiq.com/article/1522330692884)

*   [机器学习在 1 号店商品匹配中的实践 - 20170506 - 携程技术中心](https://cloud.tencent.com/developer/article/1063204)

### 待分类

**国内**

*   [**当当** 11.11：促销系统与交易系统的重构实践 - 20151113 - infoQ](https://www.infoq.cn/article/dangdang-11-11-reconstruction-system-practise)

*   [**苏宁易购** 11.11：商品详情系统架构设计 - 20151227 - infoQ](https://www.infoq.cn/article/suning-product-details-system-architecture-design?)

*   [**达观数据** 点击模型：提升算法精度的利器 - 20160315 - infoQ](https://www.infoq.cn/article/tool-to-improve-the-accuracy-of-algorithm)

*   [**达观数据** 一个可供参考的搜索引擎排序架构实践案例 - 20160830 - infoQ](https://www.infoq.cn/article/a-search-engine-scheduling-architecture-for-reference?)

*   [**达观数据** "搜你所想" 之用户搜索意图识别 - 20170608 - infoQ](http://www.6aiq.com/article/1541861015217)

*   [**链家网** 数据驱动在搜索优化与推荐策略中的实践 - 20170406 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2Fpractise-of-data-driven-search-and-optimize-in-lianjia)

*   [**豌豆荚** 发布应用内搜索协议 - 20140401 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fnews%2F2014%2F03%2Fwandoujia-search-protocol)

*   [**豌豆荚** 工程师谈其新版应用搜索技术 - 20121206 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fnews%2F2012%2F12%2Fwandoujia-app-search)

*   [**蘑菇街** 电商算法演化：从爆款模型到个性化模型（视频） - 20160523 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fpresentations%2Felectricity-business-algorithm-evolution-of-mogujie)

*   [**今日头条** 的个性化推荐 - 20150624 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Finterviews%2Finterview-with-dinghaifeng-talk-toutiao-personalized-recommendation)

*   [**艺龙** 基于实时价格计算的电商检索系统（视频） - 20160715 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fpresentations%2Felectricity-supplier-retrieval-system-based-on-real-time-price-calculation)

**国外**

*   [**Twitter** 实时搜索引擎发展历程（视频） - 20160330 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fpresentations%2Ftwitter-real-time-search-engine-development-process)

*   [**Twitter** 是怎么做搜索的 - 20160219 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Finterviews%2Finterview-with-wangtian-talk-twitter-search)

*   [**LinkedIn** 基于 Kafka 和 ElasticSearch 的实时日志分析系统 - 20170316 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fpresentations%2Flinkedin-real-time-log-analysis-system-based-on-kafka-and-elasticsearch)

*   [**Yelp** 是如何用数据驱动搜索过滤器的？ - 20151209 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fnews%2F2015%2F12%2FYelp-Search-filter)

*   [**Instagram** 的热门趋势发现算法 - 20150707 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fnews%2F2015%2F07%2FInstagram-equality)

## 开发应用

### 理论基础

*   [我爱自然语言处理](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.52nlp.cn%2F) 推荐

*   [漫话中文自动分词和语义识别](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.matrix67.com%2Fblog%2Farchives%2F4212) 膜拜中文系大牛 Matrix67

    ### 源码解读

*   [刘超觉先](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.cnblogs.com%2Fforfuture1978%2F) 详细分析了 Lucene3.x 的源码，推荐。

*   [Anatomy of an Elasticsearch Cluster: Part I](https://hacpai.com/forward?goto=https%3A%2F%2Fblog.insightdatascience.com%2Fanatomy-of-an-elasticsearch-cluster-part-i-7ac9a13b05db) - [infoQ 翻译](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2Fanalysis-of-elasticsearch-cluster-part01%3Futm_source%3Dinfoq%26utm_campaign%3Duser_page%26utm_medium%3Dlink)

*   [Anatomy of an Elasticsearch Cluster: Part II](https://hacpai.com/forward?goto=https%3A%2F%2Fblog.insightdatascience.com%2Fanatomy-of-an-elasticsearch-cluster-part-ii-6db4e821b571) - [infoQ 翻译](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2Fanatomy-of-an-elasticsearch-cluster-part02%3Futm_source%3Dinfoq%26utm_campaign%3Duser_page%26utm_medium%3Dlink)

*   [Anatomy of an Elasticsearch Cluster: Part III](https://hacpai.com/forward?goto=https%3A%2F%2Fblog.insightdatascience.com%2Fanatomy-of-an-elasticsearch-cluster-part-iii-8bb6ac84488d) - [infoQ 翻译](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2Fanatomy-of-an-elasticsearch-cluster-part03%3Futm_source%3Dinfoq%26utm_campaign%3Duser_page%26utm_medium%3Dlink)

    ### 常见问题

*   [Stackoverflow - Lucene](https://hacpai.com/forward?goto=https%3A%2F%2Fstackoverflow.com%2Fquestions%2Ftagged%2Flucene%3Fsort%3Dvotes%26pageSize%3D15)

*   [Stackoverflow - Solr](https://hacpai.com/forward?goto=https%3A%2F%2Fstackoverflow.com%2Fquestions%2Ftagged%2Fsolr%3Fsort%3Dvotes%26pageSize%3D15)

*   [Stackoverflow - Elastic](https://hacpai.com/forward?goto=https%3A%2F%2Fstackoverflow.com%2Fquestions%2Ftagged%2Felasticsearch%3Fsort%3Dvotes%26pageSize%3D15)

    ### 其他

*   [对话 Kibana 之父：如果需要，你应该自己动手编写工具 - 20170111 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fnews%2F2017%2F01%2FRashid-buildYourOwnTool)

*   [配置高性能 Elasticsearch 集群的 9 个小贴士 - 20170104 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fnews%2F2017%2F01%2FElasticSearch-9)

*   [基于 ElasticStack 的数据探索与分析 - 20161018 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Fpresentations%2Fdata-exploration-and-analysis-based-on-elasticstack)

*   [使用 Akka、Kafka 和 ElasticSearch 等构建分析引擎 - 20160825 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2Fuse-akka-kafka--build-analysis-engine)

*   [万亿级日志与行为数据存储查询技术剖析 - 20170222 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2Ftrillion-log-and-data-storage-query-techniques)

*   [谷歌的自然语言部门是啥样的？ - 20160118 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2FInside-look-of-Google-NLU-Team)

*   [通过 Baratine 将 Lucene 库暴露为微服务 - 20160225 - infoQ](https://hacpai.com/forward?goto=http%3A%2F%2Fwww.infoq.com%2Fcn%2Farticles%2FBuilding-a-Lucene-Microservice-with-Baratine)

