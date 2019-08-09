# pitfalls
踩过的坑

```
Q:
caniuse-lite is outdated.
A:
删除yarn.lock
yarn install
```

```
Q:
git设置大小写敏感
A:
git config core.ignorecase false
备份文件如果A.js
git rm A.js
将备份文件重命名a.js放到路径下
git add a.js
git commit -m '提交说明'
```
