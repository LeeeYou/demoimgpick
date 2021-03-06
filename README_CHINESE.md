# High copy WeChat image selector
包括切换文件夹、动态记录用户选中的图片、预览图片等功能

## 效果图
<img src="https://github.com/LeeeYou/LeeeYou.github.io/blob/master/images/githubpages/%E9%AB%98%E4%BB%BF%E5%BE%AE%E4%BF%A1%E9%80%89%E6%8B%A9%E5%9B%BE%E7%89%87.gif"/>

## 项目说明
这个Demo建立在 张鸿洋的博客[Android 超高仿微信图片选择器 图片该这么加载](http://blog.csdn.net/lmj623565791/article/details/39943731)
，主要修改点如下：<br>
- 1、根据用户的选择动态显示已选张数情况<br><br>
- 2、新增图片预览功能<br>
  + 2.1：预览图片入口有两个：①点击gridview图片预览区域；②点击右下角的【预览】按钮<br><br>
  + 2.2：预览图片界面可以放大、缩小图片<br><br>
  + 2.3: 预览图片界面可以选中和取消选中图片，在退出界面后“根据情况”动态刷新ImageGridShowActivity界面中图片的选中状态<br><br>
  + 2.4：上述的“根据情况”有如下两种：<br>
    - 2.4.1: 如果用户点击预览图片，只是单单预览而未做任何选中、取消选中图片的操作，则在退出界面时不会刷新ImageGridShowActivity界面
    - 2.4.2：如果用户在退出界面时选中的图片和进入界面时不同，则在退出界面时会动态刷新ImageGridShowActivity界面<br><br>
  + 2.5：预览图片界面处理OOM<br><br>
  + 2.6：监听物理返回键，动态刷新ImageGridShowActivity界面<br><br>
- 3、修改选择文件夹界面的样式<br>
  + 3.1：文件夹名称不显示问题
  + 3.2：文件名错误显示问题
  + 3.3：文件夹默认都选中问题
  + 3.4：文件夹item选择时的样式<br><br>
- 4、选中图片区域和预览图片区域的划分<br><br>
- 5、优化 createAdapter() 方法，adapter只创建一次<br><br>
- 6、文件夹和图片按照时间倒序<br><br>

## 图片选择器原型

[ppt下载链接](图片选择器原型.pptx)
