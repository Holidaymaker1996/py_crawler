# py_crawler
爬虫项目


## 功能

- 创建 Model 类，用于存放爬虫数据, 方便后续代码高效利用
- 自动爬取多页面
- 自动下载页面，提升效率及可靠性
- 浏览器翻页、下拉行为模拟，爬取动态页面
- 利用真实 cookie 通过身份验证, 爬取保护内容


## 使用方法

- 豆瓣 Top 250 Movies: 
  - 执行 douban.py
  - 运行结束后自动生成 douban.html; douban_bars.html; douban_radius.html 可在浏览器中查看
- 知乎浏览器行为模拟爬虫: 
  - 创建 serect.py 于根目录, 在浏览器中复制个人知乎账号的cookie，存放入 serect.py
  - 格式为: cookie = 'k=v;k=v;...'
  - cookie 需要去掉 _xsrf _zap  这两项
  - 执行 zhihu_bycookie.py 或zhihu_bybrowser.py
  - 无头浏览器模式可将 **# o.add_argument("--headless")** 取消注释再执行