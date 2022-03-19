# webdriver报错 + chromedriver下载
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

<img src="/images/2022-3-19-webdriver报错/chromedriver下载(1).png" width="500" height="200"/>

如上例报错中可以得知，该Chrome版本为99.0.4844.74

或者可以在Chrome浏览器中输入chrome://version/

<img src="/images/2022-3-19-webdriver报错/chrome版本.png" width="800" height="250"/>

在下载页中选择与版本相匹配的chromdriver

<img src="/images/2022-3-19-webdriver报错/chromedriver下载(2).png" width="500" height="200"/>

本人使用windows系统，因此选择windows下载包

<img src="/images/2022-3-19-webdriver报错/chromedriver下载(3).png" width="500" height="200"/>

#### 配置

<img src="/images/2022-3-19-webdriver报错/chromedriver下载(4).png" width="500" height="200"/>

将压缩包内的文件解压到python根目录下的script文件夹

<img src="/images/2022-3-19-webdriver报错/chromedriver下载(5).png" width="500" height="50"/>

## 验证
再次执行最初的代码后可顺利运行。
```
from selenium import webdriver

browser = webdriver.Chrome()
```
