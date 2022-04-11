## 前言

&emsp;&emsp;由于idea需要花钱买，对于一些学生党还是很昂贵的，但是idea有个免费30天的优惠，理论上只要我们不断去刷新那个时间就能够无限制的免费下去

## 注意

这个只针对idea的2021.2版本，因为2021.3版本需要登录才能够使用免费30天的优惠

## 步骤

- 在idea中配置第三方仓库地址

    打开 File -> Settings -> Plugins -> settings -> Manage Plugin Repositories
    新增仓库地址: https://<span><span>plugins.zhile.<span><span>io

    ![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220411204456.png)

- 安装插件
  1. 在线安装，搜索 IDE Eval Reset 插件进行安装
    ![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220411205420.png)

  2. 离线插件，[插件地址](链接：https://pan.baidu.com/s/1Ug5U-IBDDZR8W_EaauUI8A) 提取码：7b99
  
- 如何使用

  1. 点击 Help -> Eval Reset弹出来以下页面

    ![1](https://gitee.com/CX330YJ/imgs/raw/master/imgs/20220411212441.png)
页面上有用的有两个按钮和一个勾选框

  - 按钮：Reload 用来刷新界面上的显示信息。
  - 按钮：Reset 点击会询问是否重置试用信息并重启IDE。选择Yes则执行重置操作并重启IDE生效，选择No则什么也不做。（此为手动重置方式）
  - 勾选项：Auto reset before per restart 如果勾选了，则自勾选后每次重启/退出IDE时会自动重置试用信息，你无需做额外的事情。（此为自动重置方式）

这样当你每次打开idea的时候就会自动去刷新使用时间
