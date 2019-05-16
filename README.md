# TestGit
test

# 基本命令
~~~
1、git init #把这个目录变成Git可以管理的仓库

2、git add README.md #本地README.md文件添加到远程仓库

3、git add . #不但可以跟单一文件，还可以跟通配符，更可以跟目录。一个点就把当前目录下所有未追踪的文件全部add了，注意空格

4、git commit -m “注释” #把文件提交到仓库

5、git remote add origin git@github.com:Ylisen/TestGit.git #本地关联远程仓库

6、git pull --rebase origin master   

7、git clone https://github.com/Ylisen/TestGit.git   #把github上面的仓库克隆到本地

7、git push -u origin master #把本地库的所有内容推送到远程库上（第一次需要加-u，后面就不用加了）
~~~



# 绑定帐户
~~~
git config --global user.name 'yourname'
~~~

~~~
git config --global user.email 'youremail'
~~~
> 用户名和邮箱作为你的唯一标识，–global这个参数，表示这台机器上的所有Git仓库都会使用这个配置，也可以指定仓库用不同的用户名和邮箱

## 本地生成 ssh key
1. 检查是否有秘钥
~~~
cd ~/.ssh
~~~
~~~
ls
~~~

2. 如果没有的话，执行以下指令生成秘钥
~~~
ssh-keygen -t rsa -C "你的邮箱"
~~~

3. 去C:\Users\Administrator.ssh里找到id_rsa.pub，用记事本打开，全选，复制，得到ssh key公钥。    
3.1 进入github, settings      
3.2 然后打开SSH keys菜单，Add SSH key新增秘钥，填上标题（随意，建议跟repository一致），然后将id_rsa.put文件中的key粘贴，然后Add key生成秘钥。 
