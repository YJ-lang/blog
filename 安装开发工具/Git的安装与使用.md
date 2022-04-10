
# Git使用手册（idea版和vscode版）

## 准备工作

### 新建一个仓库

登陆github,点击右上角的github猫图标，点击new
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409175326.png)
填写基本信息，点击Create repository,则新的仓库创建成功.
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409175644.png)
回到仓库页面点击code获取仓库的https地址，记录下来
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409183330.png)

### 新建一个token

token在 Settings => Developer settings下，点击 Personal access tokens，点击Generate new token ,然后根据自己需求，勾选对应权限，点击Generate new，即可创建成功，切记，测试需要将创建的token复制出来保存，不然刷新页面就看不到了。

![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409175927.png)

![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409180212.png)

## idea版

### 安装

1. 新建项目，新增.gitignore文件，将不需要提交的文件配置好，点击VCS -> Create Git Repository，选择对应的文件夹
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409181947.png)

2. 将整个项目加入到Git版本控制中
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409182231.png)

3. 进行commit，填写commit Message ，点击commit，当文件从绿色变成白色表示commit成功；

4. 进行push，push 的时候点击Define remote,URL则填写你准备工作中在github上新建的仓库地址，点击push后提醒你输入登陆密码，选择token，将你新建的token填进去，推送成功，刷新你的github新建的仓库，查询推送结果
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409183051.png)

### 可能遇到的问题

#### 解决IDEA中Git无Local Changes

![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/2022-01-15-15-47-09.png)
 在LocalChanges中我们可以很清晰的看到我们修改了那些内容，如果你的界面没有这个Tab页，可以通过以下配置使其显示出来，File => Settings... =>Version Control => Commit => 将Use non-modal commit interface 勾选去掉，如图
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/2022-01-15-15-48-29.png)

#### ssl验证等问题
  
 在clone或者push代码的时候出现以下错误

 ```java
SSL certificate problem: unable to get local issuer certificate
 ```

 这是由于服务器的SSL证书未经过第三方机构签署或者使用了临时生成的SSL证书，因此无法通过Git的SSL认证导致的，可以永久取消SSL认证，步骤如下

 ```java
 //桌面右键点击 Git Bash Here
 git config --global http.sslVerify false
 ```

## vscode版

vscode已经集成了git,所以无需安装插件，主要讲如何commit和push

![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409184318.png)

然后填写提交记录

然后会出现同步，点击同步即可，这就相当于push
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409184415.png)
