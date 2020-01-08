# git提交文件到远程仓库

1. **在项目中初始化git仓库（index文件原本就存在于项目中） git init**
   
   ```text/plain
   git init
   ```
   
2. **将文件添加到缓存区（暂存区） git add**
   
   ```text/plain
	git add .
	```
   
3. **将文件传入到本地仓库 git commit**
   
   ```text/plain
   git commit -m "2020年1月8日10:25:53"
   ```

4. **上传项目到远程仓库**
    使用git remote add origin https地址确定要传输的远程仓库的地址；
    ```text/plain
    git remote add origin https://github.com/iyuyong/own
    ```
    
    使用git push -u origin master将项目推到远程仓库中

    ```text/plain    
    git push -u origin master
    ```



  > 下载远程文件到本地：
  > ```text/plain
  > git clone git@github.com:iyuyong/own.git
  > ```

# git比较本地仓库和远程仓库的差异

1. 更新本地的远程分支

   ```text/plain
   git fetch origin
   ```

2. 本地与远程的差集 :（显示远程有而本地没有的commit信息）

   ```text/plain
   git log master..origin/master
   ```

3. 统计文件的改动

   ```text/plain
   # git diff <local branch> <remote>/<remote branch>
   git diff --stat master origin/master
   ```

   

## 其他命令


git log