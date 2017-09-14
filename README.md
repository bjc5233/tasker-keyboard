# tasker-keyboard



## 说明
android上基于tasker创建的英文键盘，通过字母快速查找应用，支持拼音、黑名单
### 配置
* 安装tasker
* 导入tasker项目
* 在keyboard-init任务中配置项目根据经[KEYBOARD_ROOT_PATH]，并放入[pinying.js][jquery-3.2.1.min.js]
* 在keyboard-init任务中配置黑名单列表[apk_blacklist_names]
* 在keyboard-init任务中配置按键音效路径[KEYBOARD_SOUND_PATH]。可以使用项目sound文件夹中的几个音效
* 在keyboard-init任务中配置样式风格[KEYBOARD_STYLE]，可选值为[黑色dark\随壁纸color]；当选择color时，需要同时配置透明度[KEYBOARD_STYLE_COLOR_TRANS]，可选值为[0-1]
* [KEYBOARD_STYLE = color]需要[tasker-common](https://github.com/bjc5233/tasker-common)中的[tasker-comm-wallpaper-color]模块支持
* 执行keyboard任务，首次会提示需要生成基础数据[拼音数据、包名数据、图标数据]


---
### 使用
* 在桌面创建keyboard任务的快捷方式
* 也可以使用xposed edge模块配置[长按menu键执行keyboard任务]
* 执行快捷方式，会展示键盘界面，通过字母搜索应用，根据图标应用名选择启动
* ←表示删除一个输入字母
* ↓表示关闭该界面
* 当键盘界面已展示时，再次点击快捷方式，会关闭键盘界面

---
### 更新
* 2017-09-14版本中重写搜索和界面展示代码，加快搜索速度
* 2017-09-12版本中增加新的界面样式、注释
* 2017-08-31版本中可以提示初始化进度、增加按键音效、优化搜索效率
* 2017-08-30版本中可以展示应用图标

### 编程注意
* tasker中JavaScriptLet action中不能直接包含script关键字
```javascript
var a = "<script>xxxxx</script>";
//必须将这个关键字分隔开
var a = "<scr" + "ipt>xxxxx</scr" + "ipt>";
```

---



## 预览
<div align=center><img height="960" width="540" src="https://github.com/bjc5233/tasker-keyboard/raw/master/resources/Screenshot_2017-09-12-13-56-25-914.png"/></div>
<br>
<div align=center><img height="960" width="540" src="https://github.com/bjc5233/tasker-keyboard/raw/master/resources/Screenshot_2017-09-12-13-57-21-229.png"/></div>

---
KEYBOARD_STYLE => dark
<div align=center><img height="960" width="540" src="https://github.com/bjc5233/tasker-keyboard/raw/master/resources/demo2.png"/></div>
<div align=center><img height="480" width="270" src="https://github.com/bjc5233/tasker-keyboard/raw/master/resources/demo2.gif"/></div>
