
## 1.1. maven的安装预配置

### 1.1.1.下载maven

  [下载地址](https://maven.apache.org/download.cgi)
  ![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/ff938df7dad147dc8e2f4c4d0793adb2~tplv-k3u1fbpfcp-zoom-1.image)
  [历史版本地址](https://archive.apache.org/dist/maven/maven-3/)
  ![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220410200148.png)
  不需要下载最高版本的maven，3.6.3即可

### 1.1.2. 检查JDK版本

基本上都是1.7往上
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/a4c2e0e481d5452e8cadcdb0ea16b069~tplv-k3u1fbpfcp-zoom-1.image)

### 1.1.3. 环境变量配置

下载压缩包后解压到文件夹，然后进行环境变量配置
新建MAVEN_HOME环境变量，值为maven的根目录
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/7e0d247a29b04638bcff9c14ce5dacc8~tplv-k3u1fbpfcp-zoom-1.image)
    将MAVEN_HOME新增到path中
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/bb8d11da2eea434a8f14a3bb4411d89b~tplv-k3u1fbpfcp-zoom-1.image)

### 1.1.4. 验证是否配置成功

命令行输入，mvn -v，会出现maven基本信息
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/4c4d5f18543a4f6196a2506f006e73ac~tplv-k3u1fbpfcp-zoom-1.image)

### 1.1.5. 修改配置文件

打开配置文件（conf/settings.xml），在\<mirrors>\</mirrors>节点新增mirror子节点

```xml
    <mirror>
        <id>aliyunmaven</id>
        <mirrorOf>central</mirrorOf>
        <name>阿里云公共仓库</name>
        <url>https://maven.aliyun.com/repository/public</url>
    </mirror>
```

配置仓库地址,新增\<localRepository>\</localRepository>节点

```xml
<localRepository>E:\repo</localRepository>
```

## 1.2. idea设置maven的默认配置

由于在idea中新建项目时，会使用默认的maven版本和默认的本地仓库，解决办法如下：在File中找到Settings For New Projects,由于idea版本不一样，所以这个选项位置有所不同。我的是在这

![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/e7f8cd2058a04744bbf7d92d49a33df5~tplv-k3u1fbpfcp-zoom-1.image)
还有的是这样的
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/9b10b5cecb1f4a099cb96369d196246a~tplv-k3u1fbpfcp-zoom-1.image)
找到后，搜索maven，将maven安装路径、settings文件以及JDK路径都改成自己的电脑的地址
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/6fea053d01f14662933ae7bb97b5662b~tplv-k3u1fbpfcp-zoom-1.image)
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/6adb50bd06e5452a9cfb6d5e1eef1214~tplv-k3u1fbpfcp-zoom-1.image)
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/04c7ca3fd7b04492942a95cc04b055ed~tplv-k3u1fbpfcp-zoom-1.image)
新建一个最简单的项目，mvn clean install，可以看到下载jar包地址变成了配置的阿里云的地址了
![1](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/9712cb54cc3149f3af35c5862b29683a~tplv-k3u1fbpfcp-zoom-1.image)
说明配置成功
