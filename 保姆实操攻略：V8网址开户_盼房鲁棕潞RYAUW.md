V8网址开户【Q-——333307——】V8网址开户【 辋芷《888yx●vip》 】
V8网址开户【Q-——333307——】V8网址开户【 辋芷《888yx●vip》 】

 从0到1搭建个人技术博客：GitHub Pages + Hexo 完整指南

> 还在羡慕大牛们的个人技术博客吗？其实通过 GitHub Pages 和 Hexo，你也能在 30 分钟内搭建一个高颜值、易维护的免费博客。本文手把手教学，带你避开所有坑，建议收藏！

很多技术人都有写博客的冲动，但一想到要买服务器、配数据库、域名备案，就瞬间劝退。好消息是，用 GitHub Pages 托管静态博客，完全免费，且无需备案。

今天这篇文章，我将以 GitHub Pages + Hexo 组合为例，带你从环境准备到部署上线，走完整个流程。整个过程无需敲一行后端代码，适合所有开发者（前端、后端、运维、测试）。

 一、为什么要用 Hexo + GitHub Pages？

先来解释下这套方案的几个核心优势，这也是它成为开发者首选的原因：

1.  完全免费：博客托管在 GitHub 服务器上，无需购买云主机。
2.  极致速度：静态页面加载速度快，配合 CDN，国内访问体验尚可。
3.  版本管理：基于 Git 管理博客源文件，写文章就像提交代码，天然支持版本回滚。
4.  高度定制：主题丰富（如 Next、Butterfly），支持自定义样式和脚本。

你的角色：只需专注写好 Markdown 文件，Hexo 会自动将 `.md` 文件渲染成静态 HTML 页面。

 二、搭建前的 3 个必要条件

在开始敲命令之前，请检查你的电脑是否具备以下条件，缺一不可：

- Node.js 环境（建议 LTS 版本，自带 npm 包管理器）。
- Git 版本控制工具（用于提交代码到远程仓库）。
- 一个 GitHub 账号（用于创建仓库和开启 Pages 服务）。

如果没有安装，请先去官方下载对应版本安装，配置好环境变量。

 三、手把手实操：30分钟极速搭建

第一步：安装 Hexo 脚手架

打开终端（Mac 使用 Terminal，Windows 使用 Git Bash），输入以下命令全局安装 Hexo：

```bash
npm install -g hexo-cli
```

第二步：初始化博客目录

选一个你喜欢的本地路径，比如 `D:\\my-blog`，执行初始化命令：

```bash
hexo init my-blog
cd my-blog
npm install    安装依赖包
```

第三步：本地预览（验证是否成功）

运行 `hexo s`，浏览器访问 `http://localhost:4000`，看到默认的 Hexo 页面即代表本地环境搭建成功。（按 Ctrl + C 可停止服务）

第四步：创建 GitHub 仓库与部署

这是最关键的一步，直接决定了你的博客能否被公网访问。

1.  在 GitHub 新建仓库，仓库名必须为：`你的用户名.github.io`（注意：严格区分大小写）。
2.  回到终端，安装自动部署插件：`npm install hexo-deployer-git --save`。
3.  修改根目录下 `_config.yml` 文件，找到 `deploy` 部分，填入你的仓库地址：

```yaml
 Deployment
 Docs: https://hexo.io/docs/deployment.html
deploy:
  type: git
  repository: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

4.  最后执行部署三连：`hexo clean` -> `hexo g` -> `hexo d`。

部署完成后，稍等 1-2 分钟，打开 `https://你的用户名.github.io`，你的专属博客就上线啦！

 四、进阶优化与避坑指南

常见问题排查（必看） ：

- 部署 404：请检查仓库名是否完全匹配 `用户名.github.io` 格式。
- 样式丢失：检查 `_config.yml` 中的 `url` 和 `root` 是否填写正确。
- 新增请使用 `hexo new "文章标题"` 命令，不要手动新建 `.md` 文件。

性能优化建议：建议使用 Butterfly 主题，支持图片懒加载和 PWA 离线访问，再搭配 Giscus 评论插件，即可实现完整的博客互动系统。

 五、写在最后（互动环节）

搭建博客只是第一步，坚持输出高质量内容才是核心。我目前正在整理一套 Markdown 技术写作规范，如果你也常写技术文档，欢迎在评论区留言交流。

今日互动：你今年最想写的技术主题是什么？是微服务、中间件，还是前端可视化？在评论区立个 Flag，年底回来打卡！

如果这篇文章对你有帮助，点赞 + 在看 支持一下，让更多想写博客的朋友看到。关注我，后台回复 「部署」 获取我整理好的详细配置插件清单 PDF。

相关推荐：

https://github.com/yangpatricia1/ybxyao/blob/main/2026%E5%AE%98%E6%96%B9%E5%B9%B2%E8%B4%A7%EF%BC%9AV8%E5%9C%B0%E5%9D%80%E5%9C%B0%E5%9D%80_%E4%B9%98%E9%80%8A%E7%AF%AE%E4%BB%9D%E8%94%9AXJWDV.md

<img src="https://i.postimg.cc/2ysxGQJ5/V8-00009.png" />

相关推荐：

https://github.com/yangpatricia1/ybxyao/commit/3264d13aa213b926f870789f268d3d891068903a

<img src="https://i.postimg.cc/d0w4g90d/V8-00002.png" />
相关推荐：

https://github.com/hamiltonlinda25/thgubw/blob/main/2026%E5%AE%98%E6%96%B9%E6%B1%87%E6%80%BB%EF%BC%9AV8%E5%9C%B0%E5%9D%80app_%E6%8F%AD%E6%AE%96%E8%BF%90%E8%9B%94%E5%9C%B0FSNSN.md

<img src="https://i.postimg.cc/W4Nx0Vgy/V8-00017.png" />
相关推荐：

https://github.com/hamiltonlinda25/thgubw/commit/a607f868b1038144e4af74721427cb5fd80d3b4e

<img src="https://i.postimg.cc/5tbnDmt0/V8-00001.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
