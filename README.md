# Hello Git

## 命令

### 查看全局配置

```bash
git config --global --list
```

```bash
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
user.name=军舰
user.email=wang-junjian@qq.com
http.postbuffer=524288000
http.version=HTTP/1.1
```

### 设置全局配置

```bash
git config --global user.name "军舰"
git config --global user.email wang-junjian@qq.com
```

### 初始化仓库

```bash
git init
```
```bash
Initialized empty Git repository in /Users/junjian/GitHub/wang-junjian/HelloGit/.git/
```

### 查看状态

```bash
git status
```
```bash
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        git-command.txt

nothing added to commit but untracked files present (use "git add" to track)
```

### 添加所有文件

```bash
git add .
```

### 查看状态

```bash
git status
```
```bash
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   git-command.txt
```

### 提交

```bash
git commit -m "Init commit"
```
```bash
[main (root-commit) f0f2f20] Init commit
 2 files changed, 78 insertions(+)
 create mode 100644 README.md
 create mode 100644 git-command.txt
```

### 设置远程仓库

```bash
git remote add origin https://github.com/wang-junjian/HelloGit.git
```

### 推送本地仓库到远程仓库

```bash
# git push --set-upstream origin main
git push -u origin main
```
```bash
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 906 bytes | 906.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/wang-junjian/HelloGit.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
```


## 分支

### 查看分支

```bash
git branch
```
```bash
* main
```

### 创建分支

```bash
git branch feat-branch
```

### 交换到分支

```bash
git switch feat-branch
```
```bash
Switched to branch 'feat-branch'
```

### 创建并交换到分支

```bash
git switch -c feat-branch
```
```bash
Switched to a new branch 'feat-branch'
```
