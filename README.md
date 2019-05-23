# Robocup2019

大家在更改两个tx2上的代码之前，先切换到自己的branch，然后merge到dev分支上，示例如下：

git checkout -b lpy    (如果没有自己的分支，创建并切换到lpy分支)  /   git checkout lpy   (切换回自己的分支)

git branch  (查看当前分支，确认在自己的分支上)

git add . (添加所有更改)

git commit --author="lpy <>" -m "commit info"   (commit 并注释作者)

git checkout dev   (切换到dev分支)

git merge lpy  (将自己的更改merge到dev分支)

git checkout lpy   (切换回自己的分支)
