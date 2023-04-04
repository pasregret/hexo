# hexo 本地配置以及写博客

需要安装 git  跟 node 

安装好之后需要执行以下命令：

切换源:npm config set registry http://registry.npmmirror.com

安装hexo：npm install hexo-cli -g

初始化： hexo init
        npm install

​        

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


图片展示不出来问题：
npm install https://github.com/CodeFalling/hexo-asset-image --save 
修改node_modules 中的  hexo-asset-image index文件第58行改为 src 
_config.yml中的post_asset_folder设为true


安装bufferfix运行报错问题：
hexo安装博客踩坑：extends includes/layout.pug block content #recent-posts.recent-posts include includes/rec
安装  npm install --save hexo-renderer-jade hexo-generator-feed hexo-generator-sitemap hexo-browsersync hexo-generator-archive





 
