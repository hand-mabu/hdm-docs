# HDM官方手册
[HDM官方手册](https://hand-mabu.github.io/hdm-docs/)

## HDM文档编写教程

1. 安装 node.js
	1. [Node.js下载](http://nodejs.cn/download/)
2. 安装 hexo (一个博客框架平台)
	1. `npm install -g hexo-cli`
3. 拉取代码(以产品手册为例)
	1. `git clone -b dev https://github.com/hand-mabu/hdm-docs.git`
4. 尝试本地启动
	1. `cd hdm-docs`
	2. `hexo s` (顺利启动并打开 `localhost:4000` 便可以看到)
5. 使用 `markdown` 写法编写文档
	所有文档内容存放在 `hdm-docs/source` 根目录下，创建新文档时不需要建文件夹，所有图片放入 `source/images` 中
6. 部署流程
	1. 检查本地文档无误
	2. `cd hdm-docs`
	3. `git commit -am "[UPDATE]说明更新了哪些"`
	4. `git push origin dev`
	5. `hexo d`