## Hugo建博客流程
1. 创建一个站点 hugo new site
2. 下载主题
3. 创建文章
4. 初步配置 config. toml
5. 启动 hugo 服务器 `hugo server -D`, 进入 http://localhost:1313/ 预览页面
6. 部署到 GitHub Pages 上

### 创建站点

### 下载主题

### 创建文章
```
hugo new post/**.md
```

### 配置config.toml

### 运行Hugo

在你的站点根目录执行 `Hugo` 命令，编译生成静态文件并输出到public目录

执行`hugo server`命令，启动web服务预览

```
hugo server --theme=hyde --buildDrafts
```

浏览器里打开： http://localhost:1313

### 部署
在GitHub上创建一个Repository，命名为：coderzh.github.io

在站点根目录执行 Hugo 命令生成最终页面：

```
hugo --theme=hyde --baseUrl="http://binnote.github.io/"
```

如果一切顺利，所有静态页面都会生成到 public 目录，将pubilc目录里所有文件 push 到刚创建的Repository的 master 分支。

```
cd public
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/ywqsting/binnote.github.io.git
git push -u origin master
```

浏览器里访问：http://binnote.github.io/

git 上传本地项目 google 搜索
https://blog.csdn.net/Lucky_LXG/article/details/77849212
https://segmentfault.com/a/1190000022272311
https://www.bilibili.com/video/BV1x64y117PX?from=search&seid=4572038447049121406

## 辅助软件
- 包管理：HomeBrew/Chocolatey
- Git软件：Git
- 静态网页生成：Hugo（另外可选：Hexo，Jekyll）
- 静态网站托管：GitHub Pages，GitLab Pages，Netlify，Vercel
- 静态网页发布：Netlify，StaticGen



## 主题
- [Even](https://github.com/olOwOlo/hugo-theme-even)
- Bookworm
- Mainroad
- Binario
- hello-friend
- Loveit
- [Maupassant](https://github.com/flysnow-org/maupassant-hugo)

## 参考
- [https://github.com/gohugoio/hugo](https://github.com/gohugoio/hugo)
- [https://themes.gohugo.io/](https://themes.gohugo.io/)
- [https://github.com/topics/hugo-blog-theme](https://github.com/topics/hugo-blog-theme)