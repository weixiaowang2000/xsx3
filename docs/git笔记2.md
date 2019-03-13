## git：是一款分布式的代码版本控制工具 

## git常用命令

    查看状态：git status
    添加： git add
    提交： git commit  -m "备注"
    推送到远程：git push -u origin master
    拉取：git pull


## 删除远程添加的仓库地址

     git remote rm origin

  

## 回退版本

  一、如何查看commit_id:  

   查看日志：包括commit_id

    git log

    git reflog

二、回退版本

   1.如何回到过去: 
   
    git reset --hard 过去的commit_id

   2.如何展望未来：
   
    git reset --hard 未来的commit_id

 三、工作区，暂存区的撤消：  
    一）放弃工作区修改: git checkout -- 文件

    二）由暂存区返回到工作区 :  git reset HEAD 文件名

    三）撤消工作区的修改: git reset --hard commit_id


四、分支管理
 
   查看分支：git branch
   创建分支：git branch 新分支名
   切换分支：git checkout 要切换的分支
   推送分支到远程：git push origin 要推送的分支  例如：git push origin dev
   合并分支：git merge 要合并的分支
   删除分支：git branch -d 要删除的分支   注：合并后分支删除
   删除分支：git branch -D 要删除的分支  注：未合并后分支删除


