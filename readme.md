>写在前面：各位开发同学 我给出了一个demo模版在这里，其中通用部分的css样式建议我们使用一套，框架选择上面我们还是不强制，但是模版中后端用的是koa2，前端用的是bootstrap jquery 没有用很复杂的框架和打包工具 如果现在对后端还不熟悉的 可以直接在我这个demo上改，增加自己模块功能。   
>最后我们是要整个整合在一起，通过链接的形式。


## 证券交易系统模版

>keyword: nodejs koa2 less 

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

windows升级方式自行Google,这里略。

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
* 其中stylesheet文件夹下有我用的less文件,less文件根据文件名可以推测用途。

routes为后端提供的接口书写目录。   

bin目录下是启动文件。  

### 模版使用

我在模版中使用了less、bootstrap、jquery，都是比较基础的东西，如果大家有不了解可以直接百度搜索。

如果大家没用过express，可以考虑直接用我的这个后端框架，基本只需要改public和route两类文件。