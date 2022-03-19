# webdriver报错处理
## 问题
在使用python的selenium库的过程中，我们需要使用webdriver
```
from selenium import webdriver

browser = webdriver.Chrome()
```
此时可能出现报错
![error](/images/2022-3-19-webdriver报错/cookies报错.png)
这说明我们电脑中的Chromedriver.exe文件与Chrome浏览器的版本不匹配
## 解决方法
### 安装Chromedriver
#### 下载
下载地址: [http://chromedriver.storage.googleapis.com/index.html](http://chromedriver.storage.googleapis.com/index.html)

如上例报错中可以得知，该Chrome版本为99.0.4844.74
或者可以在Chrome浏览器中输入chrome://version/

