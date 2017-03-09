#这是我的  Alibaba Ecs 实践日志

服务器说明：
os:CentOS Linux release 7.2.1511 (Core)
bit:34


## 2017-03-09
服务器的最初目的是构建博客,考虑是用 Hexo,使用 node.js,使用 nvm 对 node.js 进行维护
1.服务器没有git，先安装git
```bash
yum install git
git config --global user.email "rhodesiax.lo@gmail.com"
git config --global user.name "rhodesiax" 
```

2.安装 vnm
```bash
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash
```
