# Git 使用教程

+ 文件状态

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





