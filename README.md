知乎用户抓取
1、爬取的数据量较多，需要使用scrapy-redis分布式框架，这里使用默认的redis指纹去重
2、考虑到各种url的结构问题，使用递归算法实现request请求发送
3、使用scrapyd对项目进行远程部署（考虑到硬件设备，只有两台从机）
4、使用mongodb做slave远程数据存储，使用redis做master主机的数据集中存放
5、使用git做好项目版本的管理
