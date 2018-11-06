# npm
> npm 是 JavaScript 的包管理工具,并且是 Node.js 平台的默认包管理工具
## 安装
>模块的依赖都被写入了package.json文件后，他人打开项目的根目录（项目开源、内部团队合作），使用npm install命令可以根据dependencies配置安装所有的依赖包
```
npm install
```
> -S, --save 安装包信息将加入到dependencies（生产阶段的依赖
```
npm install glup --save 或 npm install glup -S
```
> -D, --save-dev 安装包信息将加入到devDependencies（开发阶段的依赖），所以开发阶段一般使用它
```
npm install gulp --save-dev 或 npm install gulp -D
```
> -O, --save-optional 安装包信息将加入到optionalDependencies（可选阶段的依赖）
```
npm install gulp --save-optional 或 npm install gulp -O
```
> -E, --save-exact 精确安装指定模块版本
```
npm install gulp --save-exact 或 npm install gulp -E
```
> 本地安装
```
npm install gulp
```
> 全局安装（global）,使用 -g 或 --global
```
npm install gulp -g
```
## 卸载
```
npm uninstall [<@scope>/]<pkg>[@<version>]... [-S|--save|-D|--save-dev|-O|--save-optional]
```
> 示例： 卸载开发版本的模块
```
npm uninstall gulp --save-dev
```
## 更新
```
npm update [-g] [<pkg>...]
```
## npm init 在项目中引导创建一个package.json文件
```
npm init [-f|--force|-y|--yes]
```
## npm view 查看模块的注册信息
```
npm view [<@scope>/]<name>[@<version>] [<field>[.<subfield>]...]
```