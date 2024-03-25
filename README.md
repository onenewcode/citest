# codecov使用笔记
这里我们主要介绍github的使用教程，其它的例如Gitlab请参考 官网 https://docs.codecov.com/docs/quick-start
##  入门教程
### 注册 Codecov
官网网址，https://app.codecov.io/login 请使用github登陆，因为我们要绑定github账户进行一些信息同步。

1. 成功登录之后我们需要允许网站访问我们的github
操作如下，点击我们右上角的头像，点击 install codecov app
![img_1.png](images%2Fimg_1.png)
2. 选择我们的用户
   ![img_1.png](images%2Fimg_2.png)
3. 滑倒最下面进行授权
![img_1.png](images%2Fimg_3.png)
4. 返回codecov主页
这里便会显示我们的所有仓库
![img.png](images%2Fimg.png)
### 配置仓库
1. 我们在主页选择我们需要配置的仓库，点击configure
![img_1.png](images%2Fimg_4.png)
2. 复制密钥
点击configure我们便会进入以下界面
   ![img_1.png](images%2Fimg_5.png)
   复制步骤 1 中所示的令牌以供稍后使用。它将用于验证和验证为此存储库上传的覆盖率报告。
3. 回到github
我们需要回到github，找到我们需要添加测试的仓库，首先点击settings，然后点击左下方的secrets and variables，然后点击下方的actions
   ![img_1.png](images%2Fimg_6.png)
4. 添加密钥
点击new repository secret,然后添加我们复制的密钥，
   ![img_1.png](images%2Fimg_7.png)
   ![img_1.png](images%2Fimg_8.png)
### 添加workflow
我们接着点击github中要配置覆盖测试的仓库，点击action，
![img_1.png](images%2Fimg_9.png)
添加流文件
![img_1.png](images%2Fimg_10.png)
第二个红框中的内容需要换成你自己仓库的。然后保存我们的文件。