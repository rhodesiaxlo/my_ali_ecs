#这是我的  Alibaba Ecs 实践日志

服务器说明：
os:CentOS Linux release 7.2.1511 (Core)
bit:34


## 2017-03-09
服务器的最初目的是构建博客,考虑是用 Hexo,使用 node.js,使用 nvm 对 node.js 进行维护
1.服务器没有git，先安装git
```bash
yum install git
```
2.git 基本设置
```bash
git config --global user.email "rhodesiax.lo@gmail.com"
git config --global user.name "rhodesiax" 
```

2.安装 vnm
```bash
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash
```

执行安装脚本
```bash
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" # This loads nvm

```
验证安装
```bash
command -v nvm
```

3.安装 Node.js
```bash 
nvm install node
```

4.安装 Hexo
```bash
npm install -g hexo-cli
```

5.生成新项目,配置项目
```bash
hexo ini hexo_blog
cd hexo_blog
npm install
```

配置站点

6.发布
安装 hexo 服务器
```bash
npm install hexo-server --save
hexo server -p 80
```

The End
..
