## 基本插件

1. MyBatisCodeHelperPro (Marketplace Edition)
2. CodeGlance --缩略图
3. Alibaba Java Coding Guidelines --阿里巴巴代码规范
4. RestfulTool --URL查找 controller  RESTfultoolkit（已失效）
5. Translation --翻译
6. Maven Helper --maven冲突
7. intellij-rainbow-brackets --彩虹括号
8. .ignore --git提交忽略
9. JRebel --热部署
10. Atom Material ICons --icon插件，并不是因为图标变的有多好看，而是听说安装了这个插件后，idea会变的很丝滑（发出桀桀的笑声）

## 破解

### JRebel破解

1. 下载[激活工具](https://github.com/ilanyu/ReverseProxy/releases/tag/v1.0)（即代理工具）
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220410202343.png)

2. 运行刚才下载的可执行文件，不要关闭窗口
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220410202445.png)

3. 随机生成一个GUID，[链接](https://www.guidgen.com/)

4. 打开idea 选择Help -> JRebel -> Activation

    激活服务器地址：http://<span><span>127.0.0.1:8888/新生成的GUID
    邮箱随便填，只要是正确的邮箱格式即可
    点击Activate JRebel，即可破解成功
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220410202701.png)
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220410210123.png)

5. 选择Help -> JRebel -> Configuration ，点击 Work offline（离线模式运行）

    ![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220410210830.png)

    ![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220410210903.png)
    这里可以看到离线可使用的到期时间，现在可以关闭代理工具了，当这个时间快到了的时候可以打开代理工具重新激活插件。
