---
title: "文档站初始搭建"
date: "2026-02-11T16:40:00+08:00"
author: "PythaGodzilla"
---

## 搭建框架

文档站采用 [Hugo](https://gohugo.io/) 搭建，主要主题采用 [Hextra](https://imfing.github.io/hextra/zh-cn/)。

用 Hugo 的原因是因为我正好最近在玩 Hugo。

文档站就不费什么心思搞了。能把字放出来就好了。当然如果有后来者觉得 Hugo 限制太多要换框架也无所谓，只要别找我就行了。

但是我认为框架和主题还是不要过于modified了。

## 一些测试

关于 Hextra 这个主题，我也是第一次使用，我已经按照文档的配置配置过一遍了，感觉确实是比我自己用的 papermod 好看一些。

```python{filename="test.py"}
import numpy as np

print("Hello, World!")
```

```go {base_url="https://github.com/imfing/hextra/blob/main/",filename="docs/hugo.work"}
go 1.20
```
> 文件跳转这个讲真我真没怎么用过，好玩👍

```python {linenos=table,linenostart=42}
def say_hello():
    print("Hello!")
```

```python {linenos=table,hl_lines=[2,4],linenostart=1,filename="hello.py"}
def say_hello():
    print("Hello!")

def main():
    say_hello()
```

## 后续设计

### 图标
听说有设计好的，等到拿到了再替换。

### Console 跳转
等部署稳定了再说

### i18n
我不想做，但是我不做后续就不好做了，但是我还是不打算做。

### 评论
不可以做。我自己的网站使用了remark42，这个对接起来很轻松，而且轻量级，配置简单，支持docker部署，支持登录等等。其实如果使用我的中转服务器的话就无所谓。但是如果后续使用国内服务器要备案什么的超级麻烦，所以目前设计就不考虑评论了。真要搞上github issue吧。虽然我觉得属于是大概率也会似的地方😋

### 自定义
只打算稍微配置一下一点点css和一些layout，具体的到时候看，毕竟我用Hugo不是为了自定义的。
