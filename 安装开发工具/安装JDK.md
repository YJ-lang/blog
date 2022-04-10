
## 1. 下载JDK

- 去官网下载，[JDK历史版本下载](https://www.oracle.com/java/technologies/downloads/archive/)，但是需要注册账号登陆，不是很方便
- 网盘下载，[网盘地址,提取码：pl91](https://pan.baidu.com/s/13mkOSJ5ZtE4T7vqd5kyqRQ)
- 还有一个就是[JDK镜像网站](https://www.injdk.cn/)

## 2. 安装至指定目录

最好安装在除系统盘以外的地方

## 3. 配置环境变量

- 新建系统变量JAVA_HOME，值为JDK安装根目录
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/85b3c6d7bc0b47788a4a433d4dc6b822~tplv-k3u1fbpfcp-zoom-1.image)

- 编辑PATH变量，将刚刚新建的JAVA_HOME变量加上bin目录设置到PATH中【 %JAVA_HOME%\bin;JAVA_HOME%\jre\bin;】
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/9b5946e7291a43359ce5ca973e5ff6c4~tplv-k3u1fbpfcp-zoom-1.image)

## 4. 验证

  设置完成后，在命令行中输以下命令会出现对应的信息，如下图
  
- java -version会出现安装Java的版本信息，
  ![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/0daa8ea17557454cb19cbc90c97f96de~tplv-k3u1fbpfcp-zoom-1.image)
- 输入java
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/7b6be60edc724cf69df1c6c1db3556f0~tplv-k3u1fbpfcp-zoom-1.image)
- 输入javac
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/6d353897ed4b41cb9f7c796c504a5833~tplv-k3u1fbpfcp-zoom-1.image)
