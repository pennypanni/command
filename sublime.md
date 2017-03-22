# 目录
- [sublime](#sublime插件配置)
	-[sublime插件配置](#sublime插件配置)
	-[用命令打开sublime的配置](#subl ./ 配置)
- [iTerm安装配置](#iterm安装配置)

## sublime插件配置

**使用[Package Control](https://packagecontrol.io/installation)组件安装**

1. 按 **Ctrl+`** 调出console（注：避免热键冲突）

2. SUBLIME TEXT 3 粘贴以下代码到命令行并回车：
	```bash
	import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
	```

3. 重启Sublime Text 3

4. 如果在Perferences->package settings中看到package control这一项，则安装成功。

**用Package Control安装插件的方法**

1. 按下`Ctrl+Shift+P`调出命令面板

2. 输入`install` 调出 Install Package 选项并回车。然后搜索要安装的插件。

安装的插件： Emmet（原名 Zen Coding）、all autocomplete

## subl ./ 配置
1. `vim .bash_profile`
2. 将以下命令加入到`.bash_profile`文件中
	```bash
	alias subl=\''/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl'\'
	```
	
	添加完，保存关闭

	```javascript
	i      //在当前光标所在字符的前面插入
	Esc    //回到正常模式
	:wq    //保存并退出
	```
3. 使用`source ~/.bash_profile`，刚刚的配置会立即生效。

## iTerm安装配置

[安装主题](https://mp.weixin.qq.com/s?__biz=MzAwNzgxMjYzMA==&mid=401433562&idx=1&sn=1ca074b0629463f37a777a2b96aa98af&mpshare=1&scene=1&srcid=0222RY0edS1nmNZx6mhPYnrM&key=5c38b4f950326d7e0b9e6cffac84af8b2ef652db3e65521618f5c1575d32f39a4d2371f62c17393781e004a81ad482d1b2c2e13a0f4c11e80f0b3da9717d6f0801589b3ab3897779ec21309fef7e69c5&ascene=0&uin=MTQ5Mzc4&devicetype=iMac+MacBookPro10%2C1+OSX+OSX+10.12.3+build(16D32)&version=12020002&nettype=WIFI&fontScale=100&pass_ticket=19vyr44Wj8V%2F4eDfMX4pVbeSNA%2BgaL0uvlh2GEa9Hzg%3D)
[安装brew](https://brew.sh/)