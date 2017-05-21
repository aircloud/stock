## 证券交易系统模版

>keyword: nodejs koa less 

**重点:运行环境**

由于我后端用到了ES7的部分功能，需要保证node版本在7.0以上，npm版本在4以上。可以通过下面两个命令查看版本:

```
node --version
npm --version
```

否则需要升级版本，Mac升级方式:

```
brew uninstall node
brew install node
```

npm自动跟随升级。

*注意:如果后端不选择用koa，自行选用express的话，node可以采用低版本(比如6.3)*

### 如何运行

```
npm install
npm run start
```

然后访问`localhost:3000/example.html`

*注意:再部分电脑下目前也可以直接双击example点击打开*

### 文件组织

public为静态文件目录，所有静态资源都放在这里。    

* 其中public下example.html为我目前提供的模版。

routes为后端提供的接口书写目录。   

bin目录下是启动文件。  

### 模版使用

我在模版中使用了less、bootstrap、jquery，都是比较基础的东西，如果大家有不了解可以直接百度搜索。

如果大家没用过express，可以考虑直接用我的这个后端框架，基本只需要改public和route两类文件。