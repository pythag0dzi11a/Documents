---
title: "关于文档站"
date: "2026-02-11T17:10:00+08:00"
author: "PythaGodzilla"
weight: 4
---

## 自动交付

交付用了ssh登录，需要仓库配置secrets。

## 目录结构

参考[Hextra文件组织](https://imfing.github.io/hextra/zh-cn/docs/guide/organize-files/)。

其中每篇采用**页面包**来管理图片，例如每篇都是一个文件夹，文件夹里有index.md和图片资源等。

{{< filetree/container >}}
{{< filetree/folder name="content" >}}
{{< filetree/file name="_index.md" >}}
{{< filetree/folder name="docs" >}}
{{< filetree/file name="index.md" >}}
{{< filetree/file name="图片资源.jpg/png" >}}
{{< /filetree/folder >}}
{{< /filetree/folder >}}
{{< /filetree/container >}}

具体这样是不是最规范的或者什么命名是不是最标准的我也不知道。反正it works。

## Hugo 配置

关于 Hugo 的配置，采用的形式为[configDir](https://hugo.opendocs.io/getting-started/configuration/)

{{< filetree/container >}}
{{< filetree/folder name="content" state="closed" >}}
{{< /filetree/folder >}}
{{< filetree/folder name="config" >}}
{{< filetree/folder name="_default" state="closed" >}}
{{< filetree/file name="hugo.yaml" >}}
{{< filetree/file name="params.yaml" >}}
{{< filetree/file name="menu.yaml" >}}
{{< /filetree/folder >}}
{{< /filetree/folder >}}
{{< /filetree/container >}}
