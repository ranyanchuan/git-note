# git-note

echo "# git-note" >> README.md .   
git init .   
git add README.md .     
git commit -m "first commit" .   
git remote add origin git@github.com:ranyanchuan/git-note.git .   
git push -u origin master .   

git remote add origin git@github.com:ranyanchuan/git-note.git .  
git push -u origin master .  


#### git 远程仓库管理
1.查看当前的 remote:  `git remote -v`    
2.删除指定remote: `git remote remove <name>`  
3.添加remote: `git remote add origin git@ip:xxxgit`   


#### Mac 下如何生成SSH Key 

步骤1.检查是否已经存在SSH Key 
```js
ls -al ~/.ssh
// 如果有id_rsa 和 rsa.pub 说明存在SSH Key
-rw-------   1 ayi  staff  1675 Nov  5  2018 id_rsa   
-rw-r--r--@  1 ayi  staff   399 Nov  5  2018 id_rsa.pub
```
步骤2. 生成SSH Key (存在SSH Key 跳过)
ssh-keygen -t rsa -C "your_full_name@xxxxx.com"

步骤3. 将SSH Key添加到 GitLab 中  
复制公钥： `pbcopy < ~/.ssh/id_rsa.pub`  
添加 Key: 打开GitLab-->登录-->点击“ADD SSH KEY”-->粘贴SSH Key


 
