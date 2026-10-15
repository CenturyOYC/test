# 你好，世界。

一个简洁的中文欢迎页，使用 HTML 和 CSS 编写，无需安装依赖或构建。包含响应式布局、原创 SVG 插画、键盘导航以及减少动态效果的适配。

## 本地运行

在项目根目录执行：

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

然后在本机浏览器访问 `http://127.0.0.1:8000`。按 `Ctrl+C` 停止服务。也可以直接用浏览器打开 `index.html`。

## 文件

- `index.html`：页面内容、导航和 SVG 插画。
- `styles.css`：配色、排版和移动端样式。

修改文字和链接请编辑 `index.html`；修改配色和布局请编辑 `styles.css`。

## 验证

启动本地服务后，检查首页和样式表能正常返回：

```bash
curl --fail http://127.0.0.1:8000/ --output /dev/null
curl --fail http://127.0.0.1:8000/styles.css --output /dev/null
```

在桌面和手机尺寸下检查页面布局、键盘焦点，以及「往下看看」和 GitHub 链接。

## 发布

此项目可由任何静态网站托管服务直接发布。若使用 GitHub Pages，可在仓库的 **Settings → Pages** 中选择 **Deploy from a branch**，然后选择 `main` 分支和 `/ (root)` 目录并保存。

推送代码本身不会自动启用 GitHub Pages。
