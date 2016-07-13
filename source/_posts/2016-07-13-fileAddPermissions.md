---
title: "Mac或Liux下.sh文件添加执行权限"
subtitle: "Error:command not found"
date: 2016-07-13
author: "shijian.yang"
header-img : "linux_mac.jpg"
tags: 
	 -  Mac 
	 -  Command
---

### 前提
	1.touch hello.sh ##创建文件，mkdir：创建文件夹，内容：echo hello word
	2.sudo ./hello.sh 
	
ERROR:``command not found``  

    
### 解决方法：添加权限
``` linux
chmod +x hello.sh
```	 

#### 追記：

	#修改文件名称
 	mv hello.sh changename.sh #同一个文件夹操作为改名，不同文件夹为剪切
	#删除文件
	rm changename.sh
	#拷贝文件
	cp hello.sh test/
