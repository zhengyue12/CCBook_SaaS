# 云计算SaaS部分答案汇总

###                 云计算SaaS近年来出题主要是集中在<u>大数据开发</u>和<u>微信小程序开发</u>两个部分。在此之前你需要有一定的Java基础，和前端的知识储备（HTML，CSS，JavaScript），熟识Spring生态，JPA，微信小程序开发。

###         大数据开发分为数据采集、数据清洗、岗位聚类、岗位推荐和岗位分级聚类几个模块。数据采集主要是使用的[Web Magic](http://webmagic.io/)，WebMagic是一个简单灵活的Java爬虫框架。数据清洗是做了一些字符串规范处理的操作，具体看实际代码。岗位聚类用到了[Spark](http://spark.apache.org/)大数据框架的Kmeans聚类算法，能够调用相关的Api即可。而岗位推荐是[Mahout](http://mahout.apache.org/)推荐器的应用，不需要完成理解，同样能调用Api即可。

###         小程序开发主要是静态和动态两个方向学习，小程序静态页面和平时写网页没有特别大的区别，只要熟悉HTML，CSS，JS也就没有特别大的问题，需要注意的是小程序有几个标签存在差异，另外还要熟悉并使用[微信小程序API](https://developers.weixin.qq.com/miniprogram/dev/api/)。动态相关熟悉JPA，[Spring](http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/)，[SpringMVC](https://docs.spring.io/spring/docs/5.2.6.BUILD-SNAPSHOT/spring-framework-reference/web.html#spring-web)相关操作，熟悉其相关的注解，了解Controller、Service、Dao三层架构。后端提供接口，前端通过wx.request Api调用，具体实现自行琢磨，不再赘述。