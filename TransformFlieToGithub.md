## 在Github添加ssh公钥

+ 查看用户主目录（系统盘的Administrator）下有没有.ssh目录，如果有，再看里面是否有id_rsa和id_rsa.pub这两个文件，如果没有则需创建：

```
$ ssh-keygen -t rsa -C "xxx@xx.com"
```

+ 以记事本的方式打开id_rsa.pub文件夹并且复制.在Github-我的设置-SSH and GPG keys中添加公钥

## 在Github中创建仓库

注意:

+ **把分支名由main重命名为master**

+ **不要勾选用Readme.txt初始化仓库**

## 本地创建文件夹

```
mkdir 名称
```

## 进入文件夹

```
cd 名称
```

## 本地文件创建git文件

```
git init
```

生产.git文件夹

## 使用git命令使本地仓库与远程库连接起来

```
git remote add origin htttps://github.com/xxx/xxx.git
```

## 推送到Github仓库

```
git push -u origin master 
```

