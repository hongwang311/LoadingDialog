LoadingDialog
==
仿照ios的一个loading，但是自己太懒了，就去找了一个不维护的，感觉比较像的迁移到AndroidX，甚至连readme都是全是别人的。
--
如下是引用地址,
[GitHub - gittjy/LoadingDialog: 仿ios的加载弹窗](https://github.com/gittjy/LoadingDialog)
效果图
--
![](https://github.com/hongwang311/LoadingDialog/tree/main/demogif/自定义加载Dialog.gif)  



使用说明
--
1、项目下的build.gradle添加

```
allprojects {
		repositories {
			...
			maven { url 'https://www.jitpack.io' }
		}
	}
```
2、模块下的build.gradle添加依赖

```
dependencies {
	        compile 'com.github.gittjy:LoadingDialog:1.0.2'
	}
```
3、在代码中使用

```
LoadingDialog.Builder loadBuilder=new LoadingDialog.Builder(this)
                .setMessage("加载中...")
                .setCancelable(true)
                .setCancelOutside(true);
        LoadingDialog dialog=loadBuilder.create();
        dialog.show();
```

