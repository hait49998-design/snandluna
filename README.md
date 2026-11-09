# 霍格沃茨 · 二十一岁生日冒险

这是已整理好的完整静态网站，含四条学院路线、卢娜同行、场景配乐、官方放映入口及润色后的生日祝福。无需安装软件、运行构建或配置密钥。

## 最简单的发布方法：网页上传

1. **先解压 ZIP**，不要把 ZIP 本身上传到仓库。
2. 在 GitHub 新建一个 **Public（公开）仓库**，名字可用 `magic-birthday`，默认分支用 `main`。免费账户可用公开仓库发布 Pages。
3. 在仓库中选择 **Add file → Upload files**；空仓库可点 **uploading an existing file**。将解压后里面的所有文件和文件夹拖进去，再点 **Commit changes**。不要只上传外面的一整个父文件夹。
4. 上传后，仓库首页必须直接看到 **index.html**、**assets** 文件夹和两个 **site.开头的文件**，而不是多套一层文件夹。`assets` 必须完整上传。
5. 打开仓库 **Settings → Pages**。如果已上传 `.github/workflows/pages.yml`，在 **Build and deployment → Source** 选 **GitHub Actions**。若初次上传的运行发生在开启 Pages 之前，可到 **Actions → Publish birthday website → Run workflow** 手动运行一次。
6. 等 Actions 显示绿色成功标记后，在 **Settings → Pages** 点 **Visit site**，这里给出的就是网站地址。常见形式：`https://你的用户名.github.io/仓库名/`。

### 如果网页上传时没有带上隐藏的 .github 文件夹

这不影响网站本身。可直接在 **Settings → Pages → Source** 选 **Deploy from a branch**，分支选 **main**，文件夹选 **/(root)**，然后 **Save**。等发布完成后点 **Visit site**。

只选择其中一种发布方式即可。后续修改并提交网站文件，Pages 会按已选方式自动更新。无需使用之前的临时预览链接，也不用让自己的电脑保持开机。

## 文件说明

- `index.html`：网站首页，必须放在仓库根目录。
- `site.*.css`、`site.*.js`：当前版本的完整样式与故事程序，保留原文件名。
- `assets/`：图片及手机、平板适配版本，必须整个上传。
- `.github/workflows/pages.yml`：可选的 GitHub Actions 自动发布配置。
- `.nojekyll`：按静态文件发布的标记；使用网页上传时若漏掉，也不妨碍本网站的普通文件展示。

## 发布后检查

用手机打开网站，依次拆信、选择学院、进入第一幕。可以点“重新开始”清空此前的选择。姓名、学院和进度只保存在各自浏览器中；你测试过的进度不会随仓库发给朋友。

背景图、道具和故事本体随仓库发布；电影原声试听、YouTube 官方片段和出版社原著试读按需连接外部平台，是否能播放取决于当地网络和平台限制。无需给这些功能填写密钥，加载失败也不会阻止冒险。浏览器需要点击后才允许播放音乐。

## 图片与原作来源

这是非官方生日同人作品。哈利·波特角色与相关原作权利归各自权利人所有。官网电影剧照等素材来源已保留在网站“故事与图片来源”中；道具插画、关卡和生日对白为本作品原创改编。原著全文及电影文件未打包，放映和阅读连接原平台。此压缩包不授予第三方素材的额外使用权。

## GitHub 官方部署说明

- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages
