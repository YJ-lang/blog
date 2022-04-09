
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

- 新建项目，新增.gitignore文件，将不需要提交的文件配置好，点击VCS -> Create Git Repository，选择对应的文件夹

![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409181947.png)

- 将整个项目加入到Git版本控制中
![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409182231.png)

- 进行commit，填写commit Message ，点击commit，当文件从绿色变成白色表示commit成功；

- 进行push，push 的时候点击Define remote,URL则填写你准备工作中在github上新建的仓库地址，点击push后提醒你输入登陆密码，选择token，将你新建的token填进去，推送成功，刷新你的github新建的仓库，查询推送结果

![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409183051.png)

## vscode版

vscode已经集成了git,所以无需安装插件，主要将如何commit 、push

![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220409184004.png)

点击push后填写提交记录即可