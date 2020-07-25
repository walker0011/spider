#### 创建scrapy项目的流程

- 新建scrapy project

  ```
  scrapy startproject [project_name]
  ```

- 进入项目文件内

  ```
  cd [project_name]
  //此时出现quoteturial文件夹和scrapy.cfg文件（包含scrapy的相关部署信息）
  ```

- 创建爬虫

  ```
  scrapy genspider [spider_name] [url]
  //执行完这条命令后，在quoteturial/spiders下就会出现spider_name
  ```

  文件说明

  ```
  scrapy.cfg    : 配置文件
  items.py      :用于保存数据的数据结构
  middlewares.py：在爬取过程中定义的中间件
  pipelines.py  ：项目管道，用于输出一些settings
  settings.py   ：配置信息
  spider_name.py:核心代码
  ```

  