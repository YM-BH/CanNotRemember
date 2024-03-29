## 打标签

- 添加一个标签

```
git tag -a [标签名称] -m "描述信息"
eg：
git tag -a 3.1.4 -m "Release Version 3.1.4"
```

- 将标签提交到远程服务器上

```
git push origin --tags
```

- 切换到已有的标签

```
git checkout [标签名]
eg：
git checkout 3.1.4
```

- 删除标签

```
git tag -d [标签名]
eg：
git tag -d 3.1.4
```

- 删除远程服务器的标签

```
git push origin :refs/tags/[标签名]
eg：
git push origin :refs/tags/3.1.4
```

## 从远程分支拉取代码到本地分支

- 此方式建立的本地分支和远程分支建立映射关系

```shell
git checkout -b [本地分支名称] origin/[远程分支名称]
```

## 查看远程服务的地址

```shell
git reomote -v
```

## 修改远程服务的地址

```shell
git remote set-url origin [新的git地址]
```

## 删除远程仓库的分支

```shell
git push origin --delete [分支名称]
```

