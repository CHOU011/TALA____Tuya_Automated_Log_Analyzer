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

## 使用

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
