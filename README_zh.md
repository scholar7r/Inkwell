# Inkwell

复古、干净优雅的 Hugo 博客主题。

## 安装

要安装 Inkwell，你可以采用以下两种方式之中的任意一种，最标准的方法是使用 Submodule 方式安装，这种方式可以稳定的过渡到每一个新的版本。如果你对 Hugo 的主题编程有一定了解，并且需要对主题进行自定义操作，那么 Clone 代码仓库的安装方式更为推荐。

在下面的步骤之前，请确保你已经通过 Hugo CLI 完成了初始化。如果需要使用 Submodule 方式进行安装，请进行 Git 初始化。

### Submodule 方式安装

```shell
# 添加 Submodule
git submodule add https://github.com/scholar7r/Inkwell.git themes/inkwell

# 更新 Submodule
git submodule update --init --recursive

# Remote 更新
git submodule update --remote
```

此时 Submodule 已经在 `themes/inkwell` 目录下创建完成，接下复制 `exampleSite` 目录下的必要文件到 Hugo 目录下。

### Clone 代码仓库

```shell
# Clone 代码仓库
git clone https://github.com/scholar7r/Inkwell.git themes/inkwell
```

此时 Inkwell 仓库克隆完毕，你可以根据需求修改某些模板文件。

### 复制必要文件

主题安装完成后需要 `exampleSite` 中的部分文件复制到 Hugo 根目录下。

```
exampleSite
├── assets
├── content
├── i18n
└── hugo.toml
```

`exampleSite` 目录下包含了可自定义的 `assets`、`content` 和 i18n 文件夹，以及 hugo.toml 配置文件模板。

一般情况下你只需要将这三个文件夹和一个配置文件复制到 Hugo 根目录即可。

```shell
# 复制必要文件
cp themes/inkwell/exampleSite/* .
```

## 配置

下表列出必填项目和可修改项目，其他的项目如果在不清楚需要的情况下则不建议修改。

| 字段                   | 描述             |
| ---------------------- | ---------------- |
| baseUrl                | 网站绝对路径     |
| languageCode           | 网站使用的语言   |
| defaultContentLanguage | 网站默认语言     |
| summaryLength          | 概括文字长度     |
| copyright              | 版权声明文字     |
| favicon                | 网站图标路径     |
| author                 | 作者名称         |
| keywords               | 关键词           |
| description            | 描述             |
| logoText               | 文字 Logo        |
| links                  | 菜单栏链接       |
| title                  | 网站标题         |
| subtitle               | 网站副标题       |
| timeFormat             | 时间格式化规则   |
| enableToc              | 启用目录         |
| enableGiscus           | 启用 Giscus 评论 |
| social                 | 社交媒体图标     |
