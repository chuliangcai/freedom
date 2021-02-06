### 前言
早前进入`it`这个行业就有写博客的习惯，之前用的一款百度出的【百度空间】的产品，当时一些文章还有不少的浏览量，可惜后来【百度空间】这款产品下线了，就这样自己的一点小积累付诸东流了。后来接触到了git和github。心想不能再被别人牵着鼻子走了，写博客本地必须得留个备份，正好git满足这一点，如是就在github上间了一个个人仓库。把每次写的博客commit上去。但仓库的权限设置成了`private`，毕竟有些文章只是自己纯粹的个人笔记，不太好公开了，随着各大创作平台的兴起，掘金、简书、知乎、CSDN、还有微信公众号，其中微信公众号我觉得是一个非常不错的方式，因为只要用户关注，博主就可以给其推送文章。在知识纯粹分享的基础上加了一点强行安利的意思。那么怎么把我github上面的文章导入到微信公众号里面呢，下面就以我的这篇博文为例介绍下我是怎么操作的。
### 阻碍的地方和解决思路
* 微信公众号不支持markdown格式，这个markdown-nice这款产品可以解决
* github在线图片链接直接粘贴到微信公众号里是不能上传的会抱这个错：原因估计是因为被墙了

![image-20210206113635544](image-20210206113635544.png)

* 这点可以用`jsdelivr`进行CDN加速，比如有一张github图片地址是：`https://github.com/chuliangcai/study/blob/master/src/computer-science-education.jpg?raw=true` study是仓库名，分支是master，文件路径是`/src/computer-science-education.jpg`，加速后的地址是：`https://cdn.jsdelivr.net/gh/chuliangcai/study/src/computer-science-education.jpg`



### 开搞
1. 在github新建一个仓库，设置成`public` ，取名`freedom`寓意自由。做一个自由的👨‍💻

![image-20210206120334441](image-20210206120334441.png)

2. 使用`git clone https://github.com/chuliangcai/freedom.git` 将仓库下载到本地
3. 使用`typora` 打开`freedom`文件夹，创建好目录

![image-20210206122154575](image-20210206122154575.png)

4. 提交文章`git push`
5. 

### 附录

jsdelivr 网站地址：https://www.jsdelivr.com/?docs=gh