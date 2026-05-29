# 胡景浩 · 个人主页

基于 Marvis 官网设计语言打造的个人作品集展示页面。

## 技术栈

- 纯 HTML + CSS + JavaScript
- Three.js 3D 网状球体作品展示
- Fetch API 动态加载作品数据

## 项目结构

```
.
├── index.html      # 主页面（内嵌 CSS + JS）
├── projects.json   # 作品数据配置
└── README.md
```

## 启动方式

```bash
python3 -m http.server 8080
```

浏览器打开 `http://localhost:8080`

## 添加新作品

编辑 `projects.json`，在 `projects` 数组中追加：

```json
{
  "name": "项目名称",
  "tech": "技术栈",
  "desc": "项目描述",
  "category": "Web全栈"
}
```

可选分类：`Web全栈` `嵌入式` `AIGC`（自定义分类需在 `index.html` 中 `categoryColors` 补充颜色）。

刷新页面即可看到球体上新增的作品点。