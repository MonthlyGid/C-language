# Git 使用教程

+ 文件状态和上传到库中

  > Untracked:未识别,此文件在文件夹中，但并没有加入到git库中
  >
  > staged:暂存状态
  >
  > Unmodify:文件已经入库,未修改.
  >
  > Modified:文件已被修改可以通过git add 再次进入staged暂存状态

​       **查看文件状态命令**

       ```
          1.查看指定文件状态
          git status 文件名字
          
          2.查看所有文件状态
          git status
       ```

​       **基本git命令**

```
    1添加文件到暂存区
    git add 
    
    2添加所有文件到暂存区
    git add . 
    
    3提交暂存区的内容到本地仓库
    git commit -m "内容"
    
```

+ 忽略文件

  > 有时候有些文件是我们不想上传的，比如你的设计文件
  >
  > 那你可以在主页下建".gitgnore"文件,下面介绍文件的规则

​             **1忽略文件中的空行或以#开头的一行被忽略**

              ```
              *.txt         #忽略所有.txt格式的文件
              !lib.txt      #忽略所有.txt格式的文件,但lib.txt除外
              /temp         #仅忽略项目根目录下的TODO文件，但不包括temp
              build/        #忽略build/目录下的所有文件
              doc/*.txt     #会忽略 doc/notes.txt 但不包括doc/server/arcj.txt
              ```

+ 设置和查看git账户
  ```
  git config –global user.name ""
  git config –global user.email ""

  git config -1
  git config --system --list
  git config --global --list
  ```

+ 创建ssh公钥

  ```
  1  ssh-kengen -t rsa //会在C:\Users\Administrator\.ssh里面生成两个文件
  2  打开id_rsa.pub文件
  ```

+ Git分支

  ```
  #列出本地分支
  git branch 
  
  #列出远程分支
  git branch -r 
  
  #新建分支，但依然停留现在当前分支
  git branch [branch-name] 
  
  #新建分支，并且切换到该分支
  git checkout -b [branch] 
  
  #合并指定分支到当前分支
  git merge [branch] 
  
  #删除分支
  git branch -b [branch-name] 
  
  #删除远程分支
  git push origin --delete [branch-name]
  git branch -dr [remote/branch]
  ```


+ push

  **1.建立联系**

  > 1.git remote add origin github链接

  **2.上传**
  >1.git push -u origin main

