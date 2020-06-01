---
layout: post
title:  "Git 个人总结"
date:   2020-05-30 10:45:31 +0530
categories: ["blog", "life"]
author: "陈浩"
---
	1. 初始化：git init
	2. 添加到暂存区：git add “name”
	3. 提交到仓库：git commit -m "Adding files"
									
	4. 查看提交日志：git log
	5. 版本回退：git reset --hard HEAD~1
			git revert -n 版本号
	6. git commit 命令的-a选项可将所有被修改或者已删除的且已经被git管理的文档提交到仓库中。
			git commit -a -m "Renew"
	7. 从工作目录一步添加到仓库：git commit -am “说明”
	8. 比较暂存区域与工作目录的文件内容： git diff
分支操作：
	查看分支：git branch

	创建分支：git branch <name>
	
	切换分支：git checkout <name>或者git switch <name>
	
	创建+切换分支：git checkout -b <name>或者git switch -c <name>
	
	合并某分支到当前分支：git merge <name>
	
	删除分支：git branch -d <name>
与远程origin上的仓库进行互动:
	1、将本地的仓库提交到GitHub上：git push origin master/git push
	2、当本地仓库的时间线落后远程时需要强制：git push origin master --force
	3、将远程仓库覆盖本地仓库：git pull