# 发布到 GitHub Pages（网页操作）

1. 登录 GitHub，点击右上角 + → New repository。
2. Repository name 填 math-lab，选择 Public，点击 Create repository。GitHub Free 使用公开仓库即可发布 Pages。
3. 在空仓库点 uploading an existing file；已有文件的仓库点 Add file → Upload files。
4. 将发布包解压，把 index.html、curvature.html、sequence-limit.html、README.md、DEPLOY.md 五个文件直接拖入上传区。不要只上传 ZIP，也不要把外层文件夹整体嵌套进去。
5. 填写提交说明，例如 Add math experiments，点击 Commit changes。仓库首页应直接看见 index.html 等文件。
6. 打开仓库 Settings → Pages，在 Build and deployment 下，Source 选 Deploy from a branch；Branch 选 main，目录选 / (root)，点击 Save。若默认分支不是 main，请选择实际存放文件的分支。
7. 等待部署完成，在 Settings → Pages 查看发布网址或 Visit site；也可在 Actions 查看部署是否成功。首次发布需要等待，页面不会立刻可用。
8. 将 Pages 中显示的网址分享给别人，通常为 https://你的用户名.github.io/math-lab/ 。在线单页为同一路径下的 curvature.html 与 sequence-limit.html。
9. 后续更新：在仓库根目录再次 Upload files，上传同名新文件并提交，等待 Pages 重新部署，然后刷新在线页面。

## 常见问题

- 打开后只看到代码：访问的是 github.com 仓库文件页面；请复制 Pages 中的网站地址。
- 404：检查部署是否完成、index.html 是否位于选定发布目录、文件名大小写与网址是否一致。若仓库名改变，网站路径也要对应改变。
- 首页存在但实验打不开：确认三个 HTML 文件位于同一层，且名称与链接一致。
- 页面仍是旧版：先确认部署成功，再强制刷新浏览器缓存。
- Pages 中没有 main 可选：先上传并提交至少一个文件，再刷新设置页。

官方说明：
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
