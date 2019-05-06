# react_test
本项目是自己学习记录使用.

## 1.通过 npm 使用 React
如果你的系统还不支持 Node.js 及 NPM 可以参考我们的 Node.js 教程。

我们建议在 React 中使用 CommonJS 模块系统，比如 browserify 或 webpack，本教程使用 webpack。

国内使用 npm 速度很慢，你可以使用淘宝定制的 cnpm (gzip 压缩支持) 命令行工具代替默认的 npm:

$ npm install -g cnpm --registry=https://registry.npm.taobao.org
$ npm config set registry https://registry.npm.taobao.org
这样就可以使用 cnpm 命令来安装模块了：

$ cnpm install [name]


## 2.使用 create-react-app 快速构建 React 开发环境
create-react-app 是来自于 Facebook，通过该命令我们无需配置就能快速构建 React 开发环境。

create-react-app 自动创建的项目是基于 Webpack + ES6 。

执行以下命令创建项目：

$ cnpm install -g create-react-app
$ create-react-app my-app
$ cd my-app/
$ npm start

问题：You are running Node 5.5.0.
Create React App requires Node 8 or higher.
Please update your version of Node.
解决：node版本切换工具tnvm
查看所有的node版本：  
tnvm ls node
切换node版本：
tnvm use node-v5.5.0
nvm use node-v8.0.0

## 3.上传到代码库
Quick setup — if you’ve done this kind of thing before
or	
HTTPS
SSH
https://github.com/zhangwen0424/zw-react-app.git
Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

…or create a new repository on the command line
echo "# zw-react-app" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/zhangwen0424/zw-react-app.git
git push -u origin master
…or push an existing repository from the command line
git remote add origin https://github.com/zhangwen0424/zw-react-app.git
git push -u origin master
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.

问题：fatal: remote origin already exists.
解决：git remote rm origin
➜  my-react-app git:(master) ✗ git remote add origin https://github.com/zhangwen0424/zw-react-app.git