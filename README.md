## 基于webpack的前端工程化实践
该项目在框架上集成vue、react生态，在代码规范上集成ESLint、prettier，
在代码提交上通过git-hook库husky做提交约束，后续添加其它工程化内容
### vue工程化配置
安装webpack
安装vue@2、vue-router@3、vuex@3、axios@latest配置vue文件编译
安装less-loader、css-loader、style-loader配置less文件编译（不使用scss的原因在于sass-loader对node版本有要求，高版本在使用该sass-loader时会报错），在webpack.config.js中配置less文件时要按照顺序less-loader->css-loader->style-loader
其它工具库按需安装
### 配置编译模板
使用html-webpack-plugin这个插件在编译完成时自动生成一个html文件，同时将编译好的bundle.js通过script标签引入这个html中，使用html-webpack-plugin插件时需要指定一个模板
### 安装webpack-dev-server
配置项目热更新，指定服务执行端口
### 配置eslint、Babel
安装eslint、eslint-plugin-vue（eslint推出的对.vue文件中template、和script进行校验的插件）
在.eslintrc.js中配置
