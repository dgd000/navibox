# NaviBox

一个基于Hugo的简约、优雅的网址导航网站主题。

## 项目简介

NaviBox是一个使用[Hugo](https://gohugo.io/)框架开发的网址导航网站主题，旨在帮助用户建立自己的网址收藏夹和导航站点。该主题特点包括：

- 响应式设计，支持移动端和桌面端
- 夜间/白天模式切换
- 自定义网站分类和图标
- 一言服务集成
- 搜索功能
- 网站提交功能

## 快速开始

### 前提条件

- 安装[Hugo](https://gohugo.io/getting-started/installing/) (推荐Extended版本)
- Git

### 安装步骤

1. 创建一个新的Hugo站点（如果你还没有）:

```bash
hugo new site my-navigation
cd my-navigation
```

2. 添加NaviBox主题:

```bash
git submodule add https://github.com/shenweiyan/WebStack-Hugo themes/navibox
```

3. 修改配置文件:

```bash
cp themes/navibox/exampleSite/config.toml .
```

4. 启动Hugo服务器:

```bash
hugo server -D
```

5. 访问 http://localhost:1313 查看你的导航网站。

## 配置说明

编辑`config.toml`文件来自定义你的导航网站：

```toml
baseURL = "http://localhost:1313/"
languageCode = "zh-CN"
title = "我的网址导航"
theme = "navibox"
```

主要配置参数说明：

- `baseURL`: 你的网站URL
- `title`: 网站标题
- `author`: 作者名称
- `description`: 网站描述
- `upload`: 网站提交表单链接
- `about`: 关于导航页面链接
- `enablePreLoad`: 是否启用预加载动画
- `nightMode`: 是否默认启用夜间模式
- `yiyan`: 是否启用一言服务

## 添加网站

在`data/webstack.yml`文件中添加你的网站分类和链接。

## 贡献

欢迎提交问题和贡献代码，请通过GitHub Issues或Pull Requests参与项目。

## 许可证

本项目采用[MIT许可证](LICENSE)。

## 致谢

- 基于[WebStack-Hugo](https://github.com/shenweiyan/WebStack-Hugo)开发
- 感谢所有贡献者的支持