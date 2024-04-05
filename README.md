# Hexo博客技巧：利用JsDeliver加速文件
在你的电脑硬盘上新建一个文件夹，然后将刚建好的仓库克隆到本地 (右键Git Bash)：

git clone https://github.com/Amnesia-f/CDN.git ### 这里是你的CDN仓库地址
# 添加全部内容文件到暂存区
git add .

# 添加说明
git commit -m'第一次提交'

# 提交到远程仓库
git push
第一步add后面有个点，复制的时候不要漏了。

操作完成后你就可以直接跳到第四步了，第三步虽方式和第二步不一样，但结果是一样的。

直接上传（方法二）
新建完仓库后，选择你需要的文件上传到库中即可。

（就是这么简单粗暴）

3.调用文件
直接访问就可以了：https://cdn.jsdelivr.net/gh/你的Github用户名/你的CDN仓库名/文件文件夹/文件

例如：https://cdn.jsdelivr.net/gh/Amnesia-f/CDN@1.0/Test/1.jpg

