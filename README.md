# 测试日志分析器 · Web 版

单文件 HTML，已部署到 **GitHub Pages**，同事打开链接即可用。

## 功能

- 本地选择 `standard_*` 日志目录（不上传服务器）
- 通过率、失败分类统计
- 用例列表：搜索 / 状态筛选 / 分类筛选
- 复制失败用例 ID
- 每条用例「查看日志」：Case / Ctrl / Mod 三个 Tab
- 复制当前日志
- 下载独立 `report.html`

## 使用（本机）

用 Chrome 或 Edge 直接打开 `index.html`，或本地起一个静态服务：

```powershell
cd D:\ZZWORK\FOR_CURSOR\test-log-analyzer-web
py -3 -m http.server 8080
```

浏览器访问 `http://localhost:8080`

## 部署 GitHub Pages

1. 新建 GitHub 仓库（例如 `test-log-analyzer`）
2. 将本目录 **`index.html`** 推到仓库根目录（或 `docs/index.html`）
3. 仓库 **Settings → Pages**
   - Source: Deploy from a branch
   - Branch: `main` / `root`（或 `main` / `/docs`）
4. 等待几分钟后访问：`https://<用户名>.github.io/<仓库名>/`

## 同事怎么用

1. 打开 Pages 链接
2. 点击「选择日志目录」
3. 选中含 `testcases` 的 `standard_*` 文件夹
4. 等待分析完成，查看报告或下载 `report.html`

**推荐浏览器：** Chrome、Edge（支持选择整个文件夹）

## 日志目录结构

```
standard_20260617_190450/
  testcases/
    test_149803/
      case_log.txt
      ctrl_log.txt
      mod_log.txt
```

## 隐私说明

所有文件仅在浏览器本地读取与解析，不会上传到任何服务器。
