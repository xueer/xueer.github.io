---
layout: post
title: "Git初始化介绍3"
description: ""
category: git
tags: [git]
---
{% include JB/setup %}
## 如何提交代码到github上 ##
__________________________________
### 步骤如下: ###

#### 一、建立本地版本库 ####

1. 在本地磁盘中，建立一个文件夹，如E:\homework
1. 进入命令行窗口，指到homework目录下。
1. 输入：```git init```     (初始化）
1. 建立notepad README.md  （建立一个readme文件）
1. 输入```git add .```    (表示将当前目录下所有文件都添加到索引库中，注意：add后面有一个空格）
1. 输入```git commit -m"my first commit"``` （表示提交文件到版本库中，引号里是注释信息）
	
#### 二、配置远程版本库 ####

    E:\homework>git remote add origin https://github.com/xueer/homework.git 
注：配置库远程版本库，只需要设置一次即可.
    
#### 三、提交到github上 ####

    E:\homework>git push -u origin master  
(表示推送更新到远程版本库）
	
经过以上步骤，就可以将代码提交到github库中了。
