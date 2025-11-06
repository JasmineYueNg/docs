# Mintlify Starter Kit

Use the starter kit to get your docs deployed and ready to customize.

Click the green **Use this template** button at the top of this repo to copy the Mintlify starter kit. The starter kit contains examples with

- Guide pages
- Navigation
- Customizations
- API reference pages
- Use of popular components

[**Follow the full quickstart guide**](https://starter.mintlify.com/quickstart)

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview your documentation changes locally. To install, use the following command:

```
npm i -g mint
```

Run the following command at the root of your documentation, where your `docs.json` is located:

```
mint dev
```

View your local preview at `http://localhost:3000`.

## Publishing changes

Install our GitHub app from your [dashboard](https://dashboard.mintlify.com/settings/organization/github-app) to propagate changes from your repo to your deployment. Changes are deployed to production automatically after pushing to the default branch.

## Need help?

### Troubleshooting

- If your dev environment isn't running: Run `mint update` to ensure you have the most recent version of the CLI.
- If a page loads as a 404: Make sure you are running in a folder with a valid `docs.json`.

### Resources

- [Mintlify documentation](https://mintlify.com/docs)

---

---

当然可以 😊\
下面是一个专为 **YouWare** 定制的 `README.md` 模板（你可以直接复制到 Mintlify 编辑器里替换原来的 README 文件）。

---

````
# 🪩 YouWare Documentation Guide

欢迎来到 **YouWare 官方文档仓库**  
这里存放的是产品说明、功能介绍、用户指南与运营素材。  
本项目基于 [Mintlify](https://www.mintlify.com/) 构建。

---

## 🚀 快速开始

### 1️⃣ 本地预览文档

确保你已经安装了 Mintlify CLI：

```bash
npm i -g mint
````

在仓库根目录（含有 `docs.json` 的位置）运行：

```
mint dev
```

运行后访问：

👉 [http://localhost:3000](http://localhost:3000/)

即可在本地实时预览文档网站。

---

### 2️⃣ 编辑内容结构

所有文档页面都存放在 `/` 与子文件夹中，例如：

```
/getting-started/introduction.mdx
/guides/features.mdx
/deployment/custom-domain.mdx
```

文档导航结构由 `docs.json` 控制。\
编辑示例：

```
{
  "group": "Getting Started",
  "pages": [
    "index",
    "getting-started/introduction",
    "guides/features"
  ]
}
```

👉 保存后刷新页面即可实时看到新页面。

---

### 3️⃣ 更新并发布

1. 将修改提交到 GitHub：

   ```
   git add .
   git commit -m "update docs"
   git push
   
   ```
2. Mintlify 会自动部署（无需手动构建）。

访问你的网站地址即可看到更新内容，例如：

```
https://docs.youware.com
```

---

## 🧠 编辑规范

- 所有页面使用 **MDX** 语法，可插入组件（如 Card、Tip、Accordion 等）
- 标题使用 `#`、`##`、`###` 层级结构
- 图片放在 `/images/` 文件夹下，引用方式：

  ```
  ![界面示例](/images/ai-api-interface.png)
  
  ```
- 不同页面尽量保持统一命名结构（英文小写、用中划线分词）

---

## 🌿 SEO 与站点优化

每个 `.mdx` 页面顶部可定义 SEO 元信息：

```
---
title: "Introduction to YouWare"
description: "了解 YouWare 的核心功能与使用方式"
canonical: "https://docs.youware.com/getting-started/introduction"
---
```

同时可以在 `docs.json` 中统一配置全站主题、导航、footer 链接等。

---

## 💬 常见问题

**Q：我能否删除 API reference 文件夹？**

> 可以。如果你只写产品文档、说明书或教程，可以完全删除 `/api-reference/` 文件夹与相关配置。

**Q：文档更新多久会生效？**

> 一般在推送到主分支后 1–2 分钟内自动部署到 Mintlify。

**Q：如何绑定自定义域名？**

> 在 Mintlify Dashboard → “Add Custom Domain”\
> 输入你的域名，例如 `docs.youware.com`，并在域名解析中添加 CNAME 记录。

---

## 🧩 开发者工具

| 工具                  | 功能           | 链接                                                              |
| :------------------ | :----------- | :-------------------------------------------------------------- |
| Mintlify CLI        | 本地预览与调试      | [安装指南](https://www.mintlify.com/docs/local-development)         |
| Lucide Icons        | 文档图标库        | https://lucide.dev/icons                                        |
| Markdown Cheatsheet | Markdown语法参考 | [https://www.markdownguide.org](https://www.markdownguide.org/) |

---

## 🪄 维护信息

- **作者**：YouWare Documentation Team
- **负责人**：@Yue Ng
- **版本**：v1.0
- **最近更新**：{{ 自动更新日期 }}

---

### 🖤 感谢你的贡献

如果你在文档中发现错漏或希望添加新内容，\
请直接提交 Pull Request 或联系文档负责人。

---

```

---

是否希望我帮你扩展一个「贡献指南」部分（即 how to contribute），方便团队成员协作更新文档？
```