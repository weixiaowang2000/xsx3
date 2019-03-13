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


四、查看文件区别

    git diff 文件名

     
     + 表示新添加的代码
     - 表示删除的代码

    1.工作区区别: git diff 文件名
    2.暂存区与版本库的区别:git diff --cached 文件名
    3.工作区与版本库的区别:git diff HEAD -- 文件名
    4.查看两次版本库之间的差异：git diff commit_id commit_id

    有道云笔记git分享链接：
    
         http://note.youdao.com/noteshare?id=1d7b76b8e57e4668bf3edad1808435be
         http://note.youdao.com/noteshare?id=f7737dde1d9f20540be734f603ba5636


五、git分支【特别重要】

  查看分支：git branch
  创建分支：git branch 新分支名
  切换分支：git checkout 要切换的分支名

