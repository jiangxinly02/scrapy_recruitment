# scrapy_recruitment
用scrapy框架抓取招聘信息
10.2.1 安装
安装Scrapy in Ubuntu：
   sudo apt-get install python-dev python-pip libxml2-dev libxslt1-dev
   sudo pip install scrapy
10.2.2 制作一个Scrapy爬虫需要的四个步骤
1)新建项目 (scrapy startproject spiderName)新建一个新的爬虫项目，一个项目可能包含很多个爬虫;
scrapy startproject tencentSpider
查看项目结构：
tarena@tedu:~/Spider/tencentSpider$ tree.：
修改setttings.py 设置
			pipelines.py 保存的逻辑
			tecent.py,   抓取页面信息和继续跳转的逻辑
			items.py     保存item的映射
    3)制作爬虫 (spiders/spiderName.py)：制作爬虫开始爬取网页;
    4)存储内容 (pipelines.py)：设计管道存储爬取内容;

5)在Scrapy下启动爬虫：
scrapy crawl tencent
