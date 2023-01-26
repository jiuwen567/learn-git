# Git&GitHub的基本使用

## 初始化仓库并做最简单的配置

* cmd终端中进入想要存储代码的文件夹

* cd 到文件夹

* 使用`git init`初始化仓库 --》在当前目录下初始化本地仓库，即生成版本库(.git目录）

* ` git config --global user.name "jiuwen567"`创建用户名

* `git config --global user.email "2750826557@qq.com"`配置邮箱

* `git config --global --list`查看用户名和邮箱相关信息

  

## 设置工作区、暂存区和仓库

* 使用`git status`检测当前文件夹(需含有.git文件)状态--》增加或者删除某些东西==工作区==

* 使用`git add .`提交当前改变所有的东西(git status检测到的所有东西)或者使用`git add "文件名"`提交单个文件的改动==暂存区==

* 使用`git commit -m "自己对当前改动的解释"`==提交git仓库==

  ![image-20230126211456124](https://typora567.oss-cn-chengdu.aliyuncs.com/temp_picture/image-20230126211456124.png)

  

## 将本地仓库同步到GitHub&Gitee

### GitHub

* 创建仓库

* 将本地仓库推送给远程GitHub仓库

  ```cmd
  git remote add origin git@github.com:jiuwen567/learn-git.git
  git branch -M main
  git push -u origin main
  ```

* 配置公钥

  ![image-20230126213555784](https://typora567.oss-cn-chengdu.aliyuncs.com/temp_picture/image-20230126213555784.png)

* 获取公钥
  1. cmd中通过命令`ssh-keygen`再三次回车得到公钥
  2. 再进入到`.ssh`文件通过`explorer .`记事本打开`id_rsa.pub`查看公钥
  3. 复制粘贴公钥
* 

