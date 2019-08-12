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

```
Q:
.gitignore失效的解决办法
A:
git rm -r --cached .
git add .
git commit -m 'update'
```

```
Q:
Git误删分支恢复方法
A:
不小心删除本地分支和远程分支，使用如下方法恢复代码
git log -a 找到提交的commit id
git branch recover_branch fc4b7dca5e424207c6307118fda69215ec842555
git checkout recover_branch
```

```
Q:
npm和yarn的淘宝镜像添加
A:
npm config set registry https://registry.npm.taobao.org
npm config set disturl https://npm.taobao.org/dist
npm config set electron_mirror https://npm.taobao.org/mirrors/electron/
npm config set sass_binary_site https://npm.taobao.org/mirrors/node-sass/
npm config set phantomjs_cdnurl https://npm.taobao.org/mirrors/phantomjs/

yarn config set registry https://registry.npm.taobao.org -g
yarn config set disturl https://npm.taobao.org/dist -g
yarn config set electron_mirror https://npm.taobao.org/mirrors/electron/ -g
yarn config set sass_binary_site https://npm.taobao.org/mirrors/node-sass/ -g
yarn config set phantomjs_cdnurl https://npm.taobao.org/mirrors/phantomjs/ -g
yarn config set chromedriver_cdnurl https://cdn.npm.taobao.org/dist/chromedriver -g
yarn config set operadriver_cdnurl https://cdn.npm.taobao.org/dist/operadriver -g
yarn config set fse_binary_host_mirror https://npm.taobao.org/mirrors/fsevents -g
```
