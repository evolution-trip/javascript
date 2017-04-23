# javascript

## Day 1
### Javascript 输出

`console.log("HelloWorld!");`

### Javascript 变量
**变量是存储信息的容器。**
就好像一栋大楼里面的房子。变量名相当于门牌号，值相当于房子里装的东西。

在javascript里面，声明一个变量使用关键字`var`。例如：

`var i=10;`

`var s="Hello World!";`

`var pi = 3.1415926;`

声明一个变量时需要**注意**：

1. 变量必须以字母开头
2. 变量也能以 $ 和 _ 符号开头（不过我们不推荐这么做）
3. 变量名称对大小写敏感（y 和 Y 是不同的变量）


### Javascript 数据类型

1. 整形 `var i = 100;`
2. 浮点型 `var f = 3.14;`
3. 文本 `var s = "Hello Javascript!";`
4. 布尔 `true` `false`

JavaScript中变量有很多种类型，但是现在，我们只关注数字和字符串。
当您向变量分配文本值时，应该用双引号或单引号包围这个值。
当您向变量赋的值是数值时，不要使用引号。如果您用引号包围数值，该值会被作为文本来处理。

### Javascript 条件语句

```javascript
if(i>b){
    console.log("i is big");
}else{
    console.log("b is big");
}
```

### Git 基本命令

#### git clone
克隆现有仓库。命令格式为：`git clone [url] `。例如：

`git clone https://github.com/evolution-trip/javascript.git`

#### git add
如果当前目录下有几个文件想要纳入版本控制，需要先用 git add 命令告诉 Git 开始对这些文件进行跟踪:

`git add lsc.html`

#### git commit
将本次更新提交到本地仓库,用 -m 参数后跟提交说明的方式：
`git commit -m "sunday"`



#### git push
推送数据到远程仓库,将本地仓库中的数据推送到远程仓库。实现这个任务的命令很简单：
 `git push [remote-name] [branch-name]`
#### git pull
将远程仓库的数据抓取合并到本地。
`git pull`

#### git config
配置git

`git config --global user.email "ale0512@126.com" // 配置当前git用户的email
git config --global user.name "Your Name"
配置当前账号的用户名`

