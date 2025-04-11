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
