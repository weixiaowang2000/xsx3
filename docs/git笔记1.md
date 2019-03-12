## git是什么

   git即是一个分布式代码版本控制工具

## git使用

   第一步：如果是windows环境，先下载git客户端

     下载： https://gitforwindows.org/

   第二步：再使用git命令管理项目

      1.初始化git

         git init
    
       特点：在当前位置产生一个.git目录，用于跟踪代码
    
    2.查看状态

      git status

    3.添加文件

       git add 要添加的文件

    4.添加邮箱和用户名

    添加邮箱：
        git config --global user.email "wxw@163.com"

    添加用户名
        git config --global user.name "wxw"

        查看是否添加了邮箱和用户名：git config list


       

    5.提交到分支

      git commit -m '备注'


    6.提交到远程代码托管平台

      常用托管平台：github,gitlab,码云

        以github.com为例 提交到远程仓库

       第一步：   注册github帐号

          生成公钥密钥并把公钥

           ssh-keygen -t rsa -b 4096 -C "wxw@163.com"


           c盘/用户/用户名/.ssh下 找到id_rsa.pub打开复制全部

           添加到github.com上


    第二步：配置远程信息

       1.在远程github上创建一个存放代码的仓库
        2.连接到远程（即 开通远程索道）


          测试是否连通  ：  ssh -T git@github.com


              https://github.com/AnCrime/wxxcx.git

              git@github.com:AnCrime/wxxcx.git

         连接到远程
         git remote add origin git@github.com:AnCrime/wxxcx.git




    第三步：推送代码到远程

    

        git push -u origin master



        如果推送不上去，先拉下来：

        git pull origin master --allow-unrelated-histories




    

  

    



    


