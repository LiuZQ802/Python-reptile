# 豆瓣电影TOP250信息的爬取

本程序实现获取豆瓣电影网排名前250的电影信息

信息保存到excel表中

后续会添加函数实现保存到数据库中---已实现数据保存sqlite----后续再实现与mysql、redis交互

爬虫实现方法：

​	使用urllib库中的request获取网页HTML文档，然后用lxml库中的etree将HTML文档转换成可以用xpath操作的元素。

​	后面是用xpath定位到每一个元素，然后进行信息的筛选处理，获取影片中文名、影片外文名、影片链接、评分、评论数、概况、影片相关信息等内容