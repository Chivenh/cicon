# cicon
[![](https://img.shields.io/npm/v/cicon.svg)](https://www.npmjs.com/package/cicon)

> Cloudinsight 项目的字体文件
 
## 关于

字体库在线编辑 http://www.iconfont.cn/users/project?pid=45332

预览  https://cloudinsight.github.io/cicon/demo.html

## 安装和配置

> 假设开发环境是 `React` 和 `Webpack`

**通过 NPM 安装 `cicon` 和相关 Loader**

```sh
npm install cicon style-loader css-loader url-loader file-loader -D
```

**修改 Webpack 配置文件**

```js
module:{
  loaders:[
    {
      test:/\.css$/,
      loader:'style-loader!css-loader'
    },
    {
      test   : /\.(ttf|eot|svg|woff(2)?)(\?[a-z0-9]+)?$/,
      loader : 'url-loader?limit=999990'
    }
  ]
}
```

## 在 React 中使用

**在组件里导入字体库**

```js
import 'cicon/iconfont.css';
```

**在页面中使用样式**

```html
<i className='cicon cicon-mysql'></i>
```

## 发布流程

* 从 www.iconfont.cn 下载压缩包, 解压到项目目录, 覆盖同名文件
* **删除 iconfont.css 里的所有注释**
* 编辑 README.md
* 提交代码
* 执行 `npm run release`

## 版本历史

v1.1.0

发布到 `NPM` 

v1.0.29

```diff
+.cicon-python:before { content: "\e63c"; }
+.cicon-aliyun:before { content: "\e63d"; }
+.cicon-php:before { content: "\e63e"; }
+.cicon-java:before { content: "\e63f"; }
+.cicon-ruby:before { content: "\e623"; }
+.cicon-openstack:before { content: "\e642"; }
+.cicon-ci-large:before { content: "\e641"; }
-.cicon-ci:before { content: "\e623"; }
+.cicon-ci:before { content: "\e640"; }
-.cicon-memcache:before { content: "\e601"; }
+.cicon-memcached:before { content: "\e601"; }
```

v1.0.28

```diff
+.cicon-cacti:before { content: "\e63b"; }
```

v1.0.26

```diff
+.cicon-pubu:before { content: "\e63a"; }
```

v1.0.25

```diff
+.cicon-gunicorn:before { content: "\e638"; }
+.cicon-gearman:before { content: "\e639"; }
```

v1.0.23

```diff
+.cicon-supervisord:before { content: "\e637"; }
```

v1.0.22

```diff
+.cicon-snmp:before { content: "\e636"; }
```

v1.0.21

```diff
+.cicon-nagios:before { content: "\e634"; }
```

v1.0.19

```diff
+.cicon-iis:before { content: "\e633"; }
+.cicon-sqlserver:before { content: "\e635"; }
```

v1.0.18

```diff
+.cicon-windows:before { content: "\e624"; }
```

v1.0.17

```diff
- .cicon-onealert:before { content: "\e624"; }
+ .cicon-onealert:before { content: "\e62f"; }
```

v1.0.16

```css
.cicon-loading:before { content: "\e62f"; }
.cicon-bearychat:before { content: "\e62d"; }
```

v1.0.12

```css
.cicon-cog:before { content: "\e617"; }
.cicon-point:before { content: "\e618"; }
.cicon-oneapmlogo:before { content: "\e619"; }
.cicon-dashboard:before { content: "\e61a"; }
.cicon-desktop:before { content: "\e61b"; }
.cicon-download:before { content: "\e61c"; }
.cicon-server:before { content: "\e61d"; }
.cicon-listalt:before { content: "\e61e"; }
.cicon-ai:before { content: "\e61f"; }
.cicon-bi:before { content: "\e620"; }
.cicon-mi:before { content: "\e621"; }
.cicon-question:before { content: "\e622"; }
.cicon-ci:before { content: "\e623"; }
.cicon-onealert:before { content: "\e624"; }
.cicon-ct:before { content: "\e625"; }
```

v1.0.11

使用 [Scope](https://docs.npmjs.com/misc/scope) 发布

v1.0.10

添加了

```css
.cicon-trash:jianjiao { content: "\e616"; }
```

v1.0.9

添加了

```css
.cicon-trash:before { content: "\e614"; }
.cicon-disable:before { content: "\e615"; }
```

v1.0.8

* 必须删除css 文件中的注释，不然会出错

v1.0.7

重命名后

```css
.cicon-memcache:before { content: "\e601"; }
.cicon-php_fpm:before { content: "\e60f"; }
```

v1.0.5 

添加了

```css
.cicon-mesos:before { content: "\e612"; }
.cicon-solr:before { content: "\e613"; }
```

v1.0.1~v1.0.4 

> 不要用这几个版本

v1.0.0

```css
.cicon-apache:before { content: "\e600"; }
.cicon-memcached:before { content: "\e601"; }
.cicon-mongodb:before { content: "\e602"; }
.cicon-mysql:before { content: "\e603"; }
.cicon-ngnix:before { content: "\e604"; }
.cicon-postgresql:before { content: "\e605"; }
.cicon-redis:before { content: "\e606"; }
.cicon-tomcat:before { content: "\e607"; }
.cicon-activemq:before { content: "\e608"; }
.cicon-cassandra:before { content: "\e609"; }
.cicon-couchbase:before { content: "\e60a"; }
.cicon-couchdb:before { content: "\e60b"; }
.cicon-docker:before { content: "\e60c"; }
.cicon-elasticsearch:before { content: "\e60d"; }
.cicon-kafka:before { content: "\e60e"; }
.cicon-phpfpm:before { content: "\e60f"; }
.cicon-rabbitmq:before { content: "\e610"; }
.cicon-zookeeper:before { content: "\e611"; }
```
