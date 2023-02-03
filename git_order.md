##### 新建数据库

```
$ mkdir tutorial //新建文件夹
$ cd tutorial //进入文件夹
$ git init	//设为库
github新建仓库不要添加readme文件
```

##### 提交文件

```
$ git status //查看库目录状态
$ git add sample.txt //添加文件到索引
$ git commit -m "first commit" //提交文件
$ git log //查看历史记录
$ git log --graph --oneline //流程图查看历史记录
```

##### push到远程数据库

```
$ git remote add github https://xxxx  //remote指令添加远程数据库
$ git push github master //向远程数据库推送，master为当前分支名称
```

![image-20230203114124691](C:\Users\lixuf\AppData\Roaming\Typora\typora-user-images\image-20230203114124691.png)

从克隆库push到远程库可以直接用 git push 指令，不用加库名和分支名

##### 修改链接的远程库

git remote / git remote -v 查看远程库

git remote rm origin(name)

##### git clone

clone的库push时可以不用输入 git remote add ，直接git push origin master/main(当前分支)

##### 从远程数据库pull最新变更内容

在本地库中 

```
$ git pull <repository> <refspec>...
eg: $ git pull origin master
```

git log 查看是否更新

##### 删除远端仓库文件

```
$ rm test.txt(文件名)
$ git add test.txt
$ git commit -m ""
$ git push //更新一下就删掉了
```

