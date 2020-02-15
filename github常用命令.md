# Github 命令

### 1. 安装github
```
sudo apt-get install git
```

### 2. 进行SSH认证
```
ssh -T git@github.com
```

### 3. 配置信息

```
git config --global user.name "yuqwert"
git config --global user.email "1069153913@qq.com"
```

### 4. 查看配置
```
git config --list
```

### 5. 本地建立一个仓库
```
cd ~/Projects/git_res
git init
```

### 6. 配置ssh

#### （1）查看ssh配置
```
ls ~/.ssh
```
#### （2）创建SSH Key
```
ssh-kdygen -t rsa -C "1069153913@qq.com"
```

#### （3）验证是否来连接成功
```
ssh -T git@github.com
```

###  7. 本地仓库与github仓库关联
#### （1）关联
```
git remote add origin https://github.com/yuqwert/test_1.git
```
####  （2）移除关联
```
git remote rm origin
```
####  （3）查看关联情况
```
cat ~/Proects/git_res/.git/config
```
### 8. 建立一个说明文件
```
echo "This is version 1.0" >>~/Projects/git_res/README.txt
```

### 9.把文件添加到仓库
```
git add README.txt
commit -m "first commit"
git push -u origin master
```










