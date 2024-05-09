# 简介

一种使用内嵌浏览器和服务器端文件路径进行软件授权的实现。<br>
整体使用 Visual Basic 6.0 写成 (~~有点老，但是能用~~)<br>

# 思路

客户端：输入授权码 - 合成URL - 访问网页 - 下载文件<br>
服务端：建立授权码对应路径 - 应答请求<br>

举例：<br>
授权码：0x - 114514 - 1919810<br>
产品代码：sodayo  *(用于区分不同产品，即一个激活器可用于多个产品)*<br>
合成URL：https://ql.example.com/sodayo/0x-114514-1919810/index.html<br>
点击“授权”，软件内嵌浏览器访问对应URL，出现下载页面。<br>
【注意】使用内嵌浏览器是防止用户看到具体域名和URL，也可以直接使用系统默认浏览器打开对应URL。(o゜▽゜)o☆<br>
