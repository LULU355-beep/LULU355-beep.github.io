# VAK ChildLab GitHub Pages 部署包

必须保留在仓库根目录的文件：

- `index.html`：网站入口和全部系统代码
- `sw.js`：Service Worker，用于更新旧缓存并提供基础离线回退
- `.nojekyll`：让 GitHub Pages 直接发布静态文件

部署步骤：

1. 将上述三个文件上传到 GitHub 仓库根目录。
2. 打开仓库 `Settings` → `Pages`。
3. 在 `Build and deployment` 中选择 `Deploy from a branch`。
4. Branch 选择 `main`，Folder 选择 `/ (root)`，然后保存。
5. 发布后首次打开网站，建议强制刷新一次。
6. 如果浏览器仍显示旧版本，可刷新两次，或清除该网站的缓存和 Service Worker。

注意：不要修改 `index.html`、`sw.js` 的文件名，也不要把它们放进额外子文件夹。
