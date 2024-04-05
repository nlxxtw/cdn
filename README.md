![image](https://github.com/nlxxtw/cdn/assets/49474003/4cc1dbc8-fab2-45ee-b8a6-11ca6aa1d410)# Hexo博客技巧：利用JsDeliver加速文件
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
4.上传资源到仓库之后，需要通过 Github 自带的发布功能将文件打包才能利用 Jsdelivr 实现 CDN 加速。

点击仓库最右侧的 Release 选择新建 Create a new release
在打开的页面中填写相应的信息创建即可，记住这里创建的 Tag 名称，后续将会用到，
![image](https://github.com/nlxxtw/cdn/assets/49474003/b35cb88c-c21a-40ae-b1c0-7964c751fa88)
![image](https://github.com/nlxxtw/cdn/assets/49474003/69de7b57-a238-4705-9465-c5037ff2b8d2)
完成上述步骤之后即可通过 jsdelivr 访问仓库文件，访问地址模板如下：
https://cdn.jsdelivr.net/gh/<github-id>/<repository-name>@<tag-name>/<file-path>
如我的 Github ID 为 great-jin ，新建的资源仓库名称为 hexo-cdn ，发布的资源标签为 v-1.0 ，并在仓库中上传了 /js/text.js 文件，那么我的访问地址则为如下：
在浏览器中输入上述文件，能显示对应的文件内容则表明配置成功。
#参考https://great-jin.github.io/hexo/tool/jsdelivr/
