## 目录

- [git常用命令](#git-常用命令)
- [sublime插件配置](#sublime插件配置)
- [iTerm安装配置](#iterm安装配置)

### git 常用命令

```bash
//只克隆仓库中的一个分支
git clone -b <branch_name> <repo>

git clone -b v2 http://git.showgold.cn:8081/wabg/download.git
```

### sublime插件配置

**使用Package Control组件安装**

1. 按\` Ctrl+` \`调出console（注：避免热键冲突）

2. 粘贴以下代码到命令行并回车：
	```bash
	import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ','%20')).read())
	```

3. 重启Sublime

4. 如果在Perferences->package settings中看到package control这一项，则安装成功。

**用Package Control安装插件的方法**

1. 按下`Ctrl+Shift+P`调出命令面板

2. 输入`install` 调出 Install Package 选项并回车。然后搜索要安装的插件。

安装的插件： Emmet（原名 Zen Coding）、all autocomplete

### iTerm安装配置

[安装主题](https://mp.weixin.qq.com/s?__biz=MzAwNzgxMjYzMA==&mid=401433562&idx=1&sn=1ca074b0629463f37a777a2b96aa98af&mpshare=1&scene=1&srcid=0222RY0edS1nmNZx6mhPYnrM&key=5c38b4f950326d7e0b9e6cffac84af8b2ef652db3e65521618f5c1575d32f39a4d2371f62c17393781e004a81ad482d1b2c2e13a0f4c11e80f0b3da9717d6f0801589b3ab3897779ec21309fef7e69c5&ascene=0&uin=MTQ5Mzc4&devicetype=iMac+MacBookPro10%2C1+OSX+OSX+10.12.3+build(16D32)&version=12020002&nettype=WIFI&fontScale=100&pass_ticket=19vyr44Wj8V%2F4eDfMX4pVbeSNA%2BgaL0uvlh2GEa9Hzg%3D)
[安装brew](https://brew.sh/)
