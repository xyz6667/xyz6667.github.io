---
layout: post
title: PlantUML使用
date: 2024-05-23 15:41:25 +0800
tags: [学习使用]
toc: true
---
# 学习使用 PlantUML

## 配置
在Gemfile中添加 kramdown-plantuml
```
gem "kramdown-plantuml"
gem 'jekyll-compose', group: [:jekyll_plugins]
```
在 _config.yaml 中的 plugins 中添加
```
plugins:
  - "kramdown-plantuml"
```
随后执行命令
```
bundle install
```
最后执行，验证是否能用
```
bundle exec jekyll serve
```
## 测试
```
    ```plantuml
    a --> b
    ```
// 检验效果是否如下所示
```


```plantuml
a --> b
```