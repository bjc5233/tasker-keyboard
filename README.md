# tasker-keyboard



## 说明
android上基于tasker创建的英文键盘，通过字母快速查找应用，支持拼音、黑名单
### 配置
* 安装tasker
* 导入tasker项目
* 将pinyingMine.js、apkBlacklistName.txt[可修改为自己的黑名单]放到合适的位置
* 在tasker->keyboard-pinyin任务中修改pinyingMine.js、apkBlacklistName.txt的位置
* 首次使用需执行keyboard-init任务，来生成基础应用数据[拼音数据、包名数据、图标数据]

---
### 使用
* 在桌面创建keyboard任务的快捷方式
* 也可以使用xposed edge模块配置[长按menu键执行keyboard任务]
* 执行快捷方式，会展示键盘界面，通过字母搜索应用，根据图标应用名选择启动
* ←表示删除一个输入字母
* ↓表示关闭该界面
* 当键盘界面已展示时，再次点击快捷方式，会关闭键盘界面
* **目前搜索应用较慢，优化中**

---
### 更新
* 2017-08-30版本中可以展示应用图标


## 预览
<div align=center><img height="960" width="540" src="https://github.com/bjc5233/tasker-keyboard/raw/master/resources/demo2.png"/></div>
<div align=center><img height="480" width="270" src="https://github.com/bjc5233/tasker-keyboard/raw/master/resources/demo2.gif"/></div>
