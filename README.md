# git-note

echo "# git-note" >> README.md . 
git init . 
git add README.md . 
git commit -m "first commit" . 
git remote add origin git@github.com:ranyanchuan/git-note.git . 
git push -u origin master . 

git remote add origin git@github.com:ranyanchuan/git-note.git . 
git push -u origin master  

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
复制公钥： pbcopy < ~/.ssh/id_rsa.pub
添加 Key: 打开GitLab, 登录，找到左边栏有一个的按钮，点击“ADD SSH KEY”按钮添加，将已经获得的SSH Key粘贴到“Key”，下边的标题可以随便取，点击加入项目，这样就保持了本地与服务器端的联系.  


 
