# TestGit
test

# 绑定帐户
~~~
git config --global user.name 'yourname'
~~~

'''
git config --global user.email 'youremail'
'''
> 用户名和邮箱作为你的唯一标识，–global这个参数，表示这台机器上的所有Git仓库都会使用这个配置，也可以指定仓库用不同的用户名和邮箱

## 本地生成 ssh key
1. 检查是否有秘钥
'''
cd ~/.ssh
'''
'''
ls
'''

2. 如果没有的话，执行以下指令生成秘钥
'''
ssh-keygen -t rsa -C "你的邮箱"
'''
