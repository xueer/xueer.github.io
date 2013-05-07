---
layout: post
title: "8.git的常用命令"
description: "git的常用命令"
category: test
tags: [git]
---
{% include JB/setup %}

常用命令：

git init——创建一个git库，其实就是一个空的版本库，创建好后，在当前目录下会有一个叫.git的子目录。以后所有文件的变化信息都会保存到这个目录下。

git add——向git库添加文件，这个还可以标识文件修改，.表示当前目录下的所有文件都添加到库中。
格式：git add <path>，命令主要用于把我们要提交的文件的信息添加到索引库中。
git add .命令除了能够判断出当前目录（包括其子目录）所有被修改或者已删除的文档，还能判断用户所添加的新文档，并将其信息追加到索引中。

git commit——格式：git commit  -m "提交的描述信息"。在git commit之前最好git add，参数-m表示：指定commit（注释）信息。


git remote add origin ——格式：git remote add origin GitURL ，创建远程版本库，GitURL是github上的远程库的地址。

git push -u origin master ——将本地master推送到远端master。如果执行了git remote add origin后，以后就可以直接使用此命令自动推送到远端库中。
git push到远程的某个origin上后，使用git branch -a ,会发现，有一个origin/master的分支，origin/master指向远端的origin的master分支，
用来跟踪远程origin的master变化情况。
