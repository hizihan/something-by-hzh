# 项目开发说明

### 1、zj-wgov-ada智慧办公PC

~~~
zj-wgov-all是所有模块集合
//这个集合不发布到私服，只上传git，从git拉代码后需要执行更新指令

zj-wgov-common-fe公共组件模块

zj-wgov-doc-fe收发文模块

zj-wgov-zxsw-ada专项事务模块

zj-wgov-framework-fe外层框架源码

zj-wgov-zdysys自定义配置模块
~~~



### 2、项目搭建说明

~~~
1、安装node.js(http://www.runoob.com/nodejs/nodejs-install-setup.html)
	//选择10以上版本
2、基于node.js安装，从浙江榕基私服镜像安装依赖
	npm install -g cnpm --registry=http://39.106.38.31:8082/repository/npm-public/
	
	//如果之前安装过淘宝镜像的，可以直接切换镜像地址
	npm config set registry http://39.106.38.31:8082/repository/npm-public/
	
	//配置后可通过下面方式来验证是否成功
    npm config get registry
    
3、安装脚手架生成器
	//脚手架生成器基于yeoman编写
	//安装yeoman(已安装请忽略)，
	//（如果私服镜像安装失败请切换到淘宝镜像安装https://registry.npm.taobao.org）
	npm install -g yo
	
	//安装脚手架生成器
	npm install yo generator-modular-fe -g
	
	//更新脚手架(一般不需要更新，可跳过)
	npm install generator-modular-fe -g
	
	//使用脚手架生成器
	yo modular-fe
	
	//cd进入创建好的文件夹
	//然后安装依赖
	npm install 或者 yarn install
	
	//这里建议使用yarn install
	//在NPM 中安装yarn
	npm install -g yarn
	
	//运行项目
	npm run dev
	
4、切换私服地址
	项目搭建好，在package.json里的login和publ换成浙江榕基的地址
	稳定版本用这个：http://39.106.38.31:8082/repository/npm-releases/
	
5、发布代码到私服
	//发布代码之前要先登录
	npm run login
	
	//然后输入账号密码
	deployer
	rjadmin

	//发布代码
	npm run publ
	
6、分模块开发，更新所有用户的提交
	yarn install --no-lockfile
	
7、项目打包
	npm run deploy:build
	
~~~

//总部vpn


http://218.5.2.35/vpn.htm
kf1b
rj123456


http://192.168.210.158:6064/#/zh-CN/component/popbox
oui开发文档



