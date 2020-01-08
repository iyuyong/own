# git使用

git clone git@github.com:iyuyong/own.git

1. **在项目中初始化git仓库（index文件原本就存在于项目中） git init**
   git init

2. **将文件添加到缓存区（暂存区） git add**
   git add .

3. **将文件传入到本地仓库 git commit**
git commit -m "2020年1月8日10:25:53"

4. **上传项目到远程仓库**
  使用git remote add origin https地址确定要传输的远程仓库的地址；
  git remote add origin https://github.com/iyuyong/own

  使用git push -u origin master将项目推到远程仓库中
  git push -u origin master



## 其他命令


git log