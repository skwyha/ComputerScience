# 笔记初衷

由于每次使用Git都需要上网查找资料，故使用markdown文件记录下自己使用Git的操作，以便日后翻看。

## Git的配置

下载好Git后首先要配置好名字和Email地址，这样每次进行Git操作时才能有据可查。在Windows中打开Git Bash，而在Linux则在命令行输入：

``` shell
git config --global user.name 'your_name'

git config --global user.email 'your_email' 
```

查看配置的命令为：

``` shell
git config --list
```

## 创建仓库

接下来我们需要创建版本库(Repository),也就是代码的仓库,这个仓库里面会创建一个.git的文件夹,以便日后的数据备份和还原。

在硬盘中找一个位置,创建一个文件夹git_test作为版本库目录:

``` shell
mkdir git_test
```

输入cd git_test进入刚创建文件夹的路径:

``` shell
cd git_test
```

再输入指令git init初始化Git,告诉Git这里是一个版本库:

``` shell
git init
```

## 添加文件到Git库

在git_test目录中创建一个test.txt,内容随意。

在bash中输入命令git add “file—name”告诉Git需要追踪的文件：

``` shell
git add test.txt

```

## 删除分支

``` shell

// 删除本地分支
git branch -d localBranchName

// 删除远程分支
git push --delete origin remoteBranchName

```

## 发