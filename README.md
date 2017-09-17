# ISCO

This is just an extremely simple hugo theme. An example website can be found [here](https://zhenghe-md.github.io/)

## How to install

0. dependencies

in case you never been familiar with hugo, check the official [quick start tutorial](https://gohugo.io/getting-started/quick-start/) or if you believe me, just run the following command after you've installed [hugo](https://gohugo.io/getting-started/installing/)

```sh
$ hugo new site your_blog_name
```

1. clone this repo into your themes directory

```sh
$ cd path/to/your/hugo/site/themes && git clone 
```

2. set theme to isco in your config.toml

```
$ echo 'theme = "isco"' >> config.toml
```

now you can start the hugo dev server to see how does the site look like now:

```sh
$ hugo server -D
```

## How to customize

1. avatar

create an img directory in your static directory and put your avatar.png there

```
$ mkdir -p static/img && cp path/to/your/avatar.png static/img/
```

2. home page

copy the index.html in themes/isco/layouts and make any cutomization you need

```
$ cp themes/isco/layouts/index.html layouts/index.html
```

3. title

change title in config.toml

## Write your first post

1. create post.md
```sh
$ hugo new posts/my-first-post.md
```

2. write your post in markdown syntax

```
---
title: "My First Post"
date: 2017-09-16T22:35:10+08:00
draft: true
type: "post"
---

hello world
```

and you can add categories and tags to your blog for quick references like this

```
---
title: "JSONP是如何运作的？"
date: 2017-09-03T20:02:41+08:00
draft: false
type: "post"
introduce: "通过简单示例演示JSONP的工作方式"
categories: ["web基础"]
tags: ["http", "web"]
---
```

3. start hugo dev server to see your site

```sh
$ hugo server -D
```

4. deploy

check the official [documentation](https://gohugo.io/hosting-and-deployment/hosting-on-github/)
