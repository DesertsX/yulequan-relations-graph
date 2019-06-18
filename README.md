## 明星关系图谱
体验网址：
[https://desertsx.github.io/yulequan-relations-graph/](https://desertsx.github.io/yulequan-relations-graph/)

相关文章：
- [InteractiveGraph 实现酷炫关系图谱之前瞻](https://zhuanlan.zhihu.com/p/63221921)
- [一文教你用 Neo4j 快速构建明星关系图谱](https://zhuanlan.zhihu.com/p/61096301)

![](show.png)

使用 GitHub Pages 部署静态网页
- [部署明星关系图谱那些事儿（GitHub Pages） - “牛衣古柳”微信公众号版](https://mp.weixin.qq.com/s/l2MNAR1grDi1L6qlhHu3pA) / ["Data Analysis & Viz" 知乎专栏版](https://zhuanlan.zhihu.com/p/69398632)  
- [一文教你使用 GitHub Pages 部署静态网页 - “牛衣古柳”微信公众号版](https://mp.weixin.qq.com/s/s1MtFOU71UmUn2_TMasxHA) / ["Data Analysis & Viz" 知乎专栏版](https://zhuanlan.zhihu.com/p/69592043) 

```
# 将本地静态网页项目的文件夹变成用git管理的本地仓库
git init
# 查看所有文件，多出 .git 文件
ls -al

# 新建后对项目进行介绍
touch README.md
# 新建后可以写入后续不想提交到GitHub上的文件
touch .gitignore

# 列出所有本地分支和远程分支，仓库默认在 master 分支
git branch -a

# 新建并切换到 gh-pages 分支
git checkout -b gh-pages

# 显示有变更的文件
git status

# 删除 master 分支
git branch -d master

# 添加当前目录的所有文件到暂存区
git add .

# 提交暂存区到仓库区，并添加代码提交信息
git commit -m 'first commit'

# 添加远程仓库
git remote add origin git@github.com:DesertsX/yulequan-relations-graph.git

# 把本地的 gh-pages 分支推送到 origin 服务器上
git push origin gh-pages
```