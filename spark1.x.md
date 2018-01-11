> 看起来spark1.x 和 2.x 的版本差距还是很大的

阅读材料

* [evolution of apcahe spark](https://www.slideshare.net/datamantra/evolution-of-apache-spark)

spark2 和 1系列版本的差距行程的原因和大数据处理方式的演进有很大的关系。


### 2014

* 比较流行 Pig, Hive 来进行数据处理
* 数据源一般是RDBMS，然后倒入到 Hive中，所以很多case都是基于结构化数据的
* 效率是比较低的

起初的 spark 版本更多的是支持结构化数据的导入，多种数据库


### 演化

* 起初的 saprk 内存cache使用的是 java 字节码
* Flink 这样的工具开始使用自己管理内存的策略，当时的spark还是使用 JVM 来管理，后来 spark 也跟上，使用这种策略(1.4版本), 减少了 vm 大小和 GC 时间对时间的影响
* spark 开始有自己的大数据处理 DSL (1.6版本)


