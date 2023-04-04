# hexo 本地配置以及写博客

需要安装 git  跟 node 

安装好之后需要执行以下命令：

切换源:npm config set registry http://registry.npmmirror.com

安装hexo：npm install hexo-cli -g

初始化： hexo init
        npm install
        
    hexo g  hexo s  本地运行
    hexo d 到github 需要配置git ssh

生成 ssh：
1、git config --global user.name "Name"
   git config --global user.email "Email"

2、 ssh-keygen -t rsa -C "Email"

3、位置：  ~/.ssh/id_rsa.pub 

4、配置到github

_config.yml 配置：
deploy:
  type: git
  repository: git@github.com:dingxind/dingxind.github.io.git
  branch: master
  
安装扩展：
npm i hexo-deployer-git

新建博客： hexo new post "article title"






 
