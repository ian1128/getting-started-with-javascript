## 使用说明

编程小白再进行操作之前请注意三点。

1. 指令的构成，该空格的要空格。
```
// 错误
> xcode-select--install // select后面没有空格

// 正确
> xcode-select --install // select后面有空格
```

2. 双引号要用英文
```
// 错误
> git commit -m “这是一次提交” // 用了中文的引号”“

// 正确
> git commit -m "这是一次提交" // 要用英文""
```

3. 终端常用指令总结

[mac终端](https://github.com/xugy0926/getting-started-with-javascript/blob/master/topics/MAC-Terminal-command-list.md)
[win终端](https://github.com/xugy0926/getting-started-with-javascript/blob/master/topics/Win-Command-list.md)


## 开始

还记得上一篇【第一次使用git】吗？这一次我们发起一次pull request。

当我们要协同工作的时候。一定会有一个人先建立一个新项目（命名为项目A），其他开发者会fork项目A到各自的仓库。

现在假设有一个工程师fork了项目A到自己的仓库（fork后的项目暂且叫项目B）。这个工程师就会把项目B clone到本地开始工作，然后把修改提交并推送到远程的项目B。

工作完成后，这个工程师就想把自己提交到项目B的内容合并到项目A里，怎么办呢？这时就要发起一次pull request。

当项目A的负责人收到你的pull请求时，就会进行merge动作。

下面就教你怎么操作pull request。在进行操作之前，请先看一下项目[words-from-the-heart](https://github.com/xugy0926/words-from-the-heart)的项目说明。 

通过下面的操作，我希望我们一起完成一件有意思的事情。

#### 1. fork项目words-from-the-heart

在项目 [words-from-the-heart](https://github.com/xugy0926/words-from-the-heart) 页面，点击【fork】。

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/fork.png)

正在fork时，你会看到这个页面

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/forking.png)

#### 2. clone项目到本地

fork成功，在你的github主页会多出一个项目words-from-the-heart。请注意，这个words-from-the-heart项目已经明确是你自己的。

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/my-fork.png)

这时，你就可以clone你的words-from-the-heart。因为是你的words-from-the-heart项目，请把下面<your project url>替换成你的项目url。

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/words-form-the-heart-url.png)

```
// 用https的url
> git clone <your project url>
```

#### 3. 修改文件

1. 在words-from-the-heart文件夹，添加一个json格式文件，文件命名为你的名字。比如:xugaoyang.json。其实，你可以拷贝template.json后再修改你拷贝的文件名即可。（千万别直接改我的template.json，也别修改其他任何文件，否则我会拒绝你的pull request请求的）
2. 修改xugaoyang.json里的内容。文件里有三个内容需要填写：头像链接，姓名，心里话。只修改双引号里面的内容即可。
3. 头像链接如何获取？你需要把头像上传到网上，我介绍一款图床给你，把图片上传到图床上，就能拿到一个url。https://toolinbox.net/iPic/

关于图床，事实上QQ空间，百度云盘，微博都可以成为你放图片的地方，只要你懂怎么拿到url即可。

为了保证我在制作html页面的美观度，图片尽量用微信头像。如果你担心隐私问题，也请用和微信头像同样长宽比的图片。

#### 4. 查看状态

查看修改状态，每个人只能有一个增加的json文件。否则，我最后会拒绝你的pull request请求。

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/git-status.png)

```
> git status
```

#### 5. 添加修改

```
> git add -A
```

#### 6. 提交修改

```
> git commit -m "你的提交说明"
```
#### 7. 推送到远程

```
> git push origin master
``` 

#### 8. 发起pull request

在github中，进入你words-from-the-heart的项目发起pull request, 选择【Pull requests】标签，点击【New pull request】。

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/my-fork.png)

点击【Create pull request】

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/pull-request-2.png)

点击【Create pull request】

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/pull-request-3.png)

看到下面的页面，就说明你pull request成功了

![](https://raw.githubusercontent.com/wiki/xugy0926/getting-started-with-javascript/pull-request-4.png)

## 结束语

1. 我会把你们的提交merge到我的项目中。
2. 所有数据将做成一个页面供我们一起留念。

