# HDM官方手册编写教程


* **安装 node.js**
	* [Node 官网地址](http://nodejs.cn/download/)
* **安装 hexo** (一个博客框架平台)
  * 安装 `hexo`


            npm install -g hexo-cli

    
  * 拉取代码(以产品手册为例)


            git clone -b dev https://github.com/hand-mabu/hdm-docs.git

  
  * 尝试本地启动
    
            cd hdm-docs
            hexo s (顺利启动并打开localhost:4000便可以看到)

	   
* **使用 markdown 写法编写文档**

    所有文档内容存放在 `hdm-docs/source` 根目录下，创建新文档时**不需要建文件夹**，所有图片放入 `source/images` 中
    
* **部署流程**
	* 检查本地文档无误
	* `cd hdm-docs` ---进入文档文件夹
	* `git commit -am "[UPDATE]说明更新了哪些"` ---commit修改请求 如果不行还请先 `git add .` `git commit -m "..."`
	* `git push origin dev` ---提交代码到dev分支
	* `hexo d` ---提交代码到master