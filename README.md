# Kook自用美化css备份

自从开黑啦更新为kook后就不打算在更新这个样式了，弄起来也挺废时间的。不过居然没想到居然还有小伙伴在用这个样式，索性就继续更新一下吧

## 开始之前请注意

* 库中的`index.htm`文件为样板文件，请勿用做替换你本地`index.htm`文件使用

* 请于kook外观设置中将主题模式切换为`暗黑模式`，然后关闭`自动切换主题模式`

## 使用方式

1. 将下载得到的`static`文件夹放入`kook安装目录\resources\app\webapp\build`（如果提示是否覆盖则直接覆盖）

2. 在`kook安装目录\resources\app\webapp\build\static\videos`文件夹中放入要用作背景的MP4视频文件（最好为16：9），然后记住视频文件名

3. 用你喜欢的文本编辑器打开`kook安装目录\resources\app\webapp\build\index.htm`(如果怕修改错误可以先备份一下)。
   找到行`<noscript>You need to enable JavaScript to run this app.</noscript>`,在它后面加上如下代码：
   
   ```html
     <!--自定义样式-->
     <link href="/app/static/css/kook.video.css" rel="stylesheet">
     <div id="bg">
         <video id="v1" autoplay loop muted>
             <source src="/app/static/videos/filename.mp4" type="video/mp4"  />
         </video>
     </div>
     <!--自定义样式-->
   ```
   
   其中`filename.mp4`替换为前面记住的视频文件名

4. 随后重启kook

效果预览：      
![动画.gif](https://s2.loli.net/2022/07/17/gaLR7Tfr69AF5Jl.gif)

## 一些其他的东西

1. 该样式仅供学习交流使用，请勿用作它途

2. 有问题请到[我的kook服务器](https://kook.top/8yNFIi)反馈，github这边我不经常看
