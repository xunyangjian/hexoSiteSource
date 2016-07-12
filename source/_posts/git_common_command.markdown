---
layout:     post
title:      "Git常见问题及命令"
subtitle:   ""
date:       2016-07-12
author:     "shijian.yang"
header-img: "git-right.jpg"
catalog :   true
tags:
    -  Source Manage
    -  Git
---

### 持续更新中

 ### 1.创建分支并上传远程 
 _命令_
    
 >		1. git checkout -b new_branch_name
 >		2. git push -u <remote_name> <branch_name>
 ---

 ### 2.checkout 远程分支并跟随
 _命令_
 >      git chekcout -b <local_checek_name> --track <remote/branch_name>

 > **说明**
 > 1. `跟随`：分支从远程仓库checkout之后会默认跟随分支，`git push`执行若不指定分支，会提交到跟随的分支；
 > 2. `--track`:跟随；
 > 3. `--no-track`: 不跟随；

 ---


 ### 3.windows下项目文件路径过深，产生如下错误
 _命令_
 >      git config core.longpaths true

 ---
 ### 4.添加系的远程仓库
 _命令_
 >		git remote add <name> <remote_url>
 >		git remote -v //显示全部remote

 ---
 ### 5.ERROR: fatal: Cannot update paths and switch to branch 'XXXX' at the same time.
 **说明**

  若没本地有checkout分支的索引时，出现上面的权限；

  解决方法：git fetch <remote> [branch name]

 ---
 ### 6.checkout单个文件从让其他源 
 _命令_
 >		git checkout <reomte/branch> --<path/to/you want/file>

 ---
 ### 7.local branch 制定跟随远程分支
 _命令_
 > 		git branch -u <remote/branch> <local_branch_name>
 例如：   git branch -u   rontech/customer-search   customer-search

 ---

