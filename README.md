# Pull Request 流程
当前用户是zhenhappy,在本地新建一个目录Pull-Request-Demo,并初始化git

    mkdir Pull-Request-Demo;cd Pull-Request-Demo;git init
这时会在Pull-Request-Demo目录里面生成一个.git的隐藏目录
接下来编辑README文件,并提交版本h1


    vim README;git add .;git commit

![enter description here][1]

再次有修改后提交版本h2

    edit,edit;git commit

![enter description here][2]

绑定远端仓库并Push

    git remote add origin git@github.com:zhenhappy/Pull-Request-Demo.git
    git push origin master

![enter description here][3]

然后切换到用户q505507538, 去Fork用户zhenhappy的项目
然后克隆到他本地

    git clone git@github.com:q505507538/Pull-Request-Demo.git

这时用户q505507538这边也有h1,h2这两个版本
新建一个分支add_logo

    git checkout -b add_logo

![enter description here][4]

这时候继续编辑修改,得到L1,L2两个版本

    edit,edit;git commit

![enter description here][5]

Push到远端仓库

    git push origin add_logo

然后在Github上面就会出现一个Compare & pull request的按钮

![enter description here][6]

点击Compare & pull request按钮,填写备注提交即可

![enter description here][7]

切换回zhenhappy用户, 去接收这个Pull Request
但是实际的开发可能会更复杂,可能在接收这个Pull Request的时候已经有版本提交了,这时候在zhanhappy这边提交一个h3的版本

    edit,edit;git commit

![enter description here][8]






  [1]: ./images/1443077250671.jpg "1443077250671.jpg"
  [2]: ./images/1443077332128.jpg "1443077332128.jpg"
  [3]: ./images/1443077702234.jpg "1443077702234.jpg"
  [4]: ./images/1443080775460.jpg "1443080775460.jpg"
  [5]: ./images/1443080824333.jpg "1443080824333.jpg"
  [6]: ./images/1443083207465.jpg "1443083207465.jpg"
  [7]: ./images/1443083278023.jpg "1443083278023.jpg"
  [8]: ./images/1443083515886.jpg "1443083515886.jpg"
