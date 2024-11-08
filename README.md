## 原理
通过控制浏览器翻页的方式获取书籍内容并保存到本地。

## 使用方法

1. 安装jdk，jdk版本11以上，过程略。
2. 下载ChromeDriver，和jdread-downloader.jar放在同一目录。ChromeDriver大版本要等于你安装的chrome版本，比如chrome 110就得用ChromeDriver 110版本（有三个下载链接，如下）。
3. 114及更早版本：
chromedriver.storage.googleapis.com/index.html；
113及113以后下载（json页面）
googlechromelabs.github.io/chrome-for-testing/known-good-versions-with-downloads.json
130及以后
https://googlechromelabs.github.io/chrome-for-testing/
4. 在jar文件所在目录打开终端，运行jar包：`java -jar jdread-downloader.jar`
5. 运行后会自动打开chrome，并跳转到登录页面，登录后打开书籍的第一页，向下滚动页面直至能看到“下一章”的按钮
6. 回到命令行窗口输入任意字符按回车开始爬取，爬取完成后会生成HTML页面，如果想离线保存图片的话可以用浏览器打开然后右键另存为完整的HTML文件。
7. 操作浏览器打开下一本书的封面，重复上一个步骤。
