---
title: "Hugo"
date: 2025-05-07T22:49:07+08:00
draft: false
---

## 官网(official site)
https://gohugo.io/

- 安装hugo

* ubuntu
```
sudo snap install hugo
```

- 新建自己的blog站点

```Shell
hugo new site quickstart
```

- 下载theme

[https://themes.gohugo.io/](https://themes.gohugo.io/)

```Shell
cd quickstart
git init
git submodule add https://github.com/mrmierzejewski/hugo-theme-console.git themes/console
```

- 应用theme

打开site下的config.toml，追加theme属性

```Shell
baseURL = 'http://example.org/'
languageCode = 'en-us'
title = 'My New Hugo Site'
theme = 'console'

```

- 新增内容

```Shell
hugo new content/posts/my-first-post.md
```

- 启动服务

```Shell
hugo server -D
```

[Deploy to github](https://flowus.cn/d353d4ba-116e-4af9-9f35-363fcf8c8e63)


