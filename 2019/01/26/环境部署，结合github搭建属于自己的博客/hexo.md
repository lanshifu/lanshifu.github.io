#### 一、参考
[参考](https://blog.csdn.net/weixin_39879178/article/details/80319392)

#### 二、准备
1.安装Node.js [下载](https://nodejs.org)
2.git，应该没问题

#### 三、检查环境
>node -v
>npm -v
>git --version

#### 四、github 配置ssh
配置省略。。。

检查ssh key是否配置成功
>ssh -T git@github.com

#### 五、全局配置设置到淘宝源
>npm config set registry https://registry.npm.taobao.org


#### 安装hexo插件，，阿里云源 大概10s安装
>npm install hexo-cli -g 

如果报错npm权限问题
>sudo chown -R $USER /usr/local 

#### 初始化
>hexo init Hexo 
cd /Hexo 
npm instal 
hexo generate（可简写为hexo g） 

#### 启动服务
>hexo sever（可简写为hexo s）


![17795f635218ca1b59e330fad27f86d0.png](evernotecid://A8603FB7-398F-4DB3-B5AF-F4E62E30CFD9/appyinxiangcom/21961528/ENResource/p21)

发现到最后已经有网址，复制+粘贴到浏览器访问

大于hexo 3.0的上传到github的方法： 

#### 安装部署到github插件依赖
>npm install --save hexo-deployer-git

#### 关联github
修改 *\_config.yml* 文件
>deploy:
  type: git
  repository: git@github.com:lanshifu/hexo.git
  bransh: master
  

#### 本地增加博客
>hexo new "file.md"

#### 生成文件夹
>hexo generate

#### 同步到github
>hexo deploy


#### 修改主题
下载
>https://hexo.io/themes/