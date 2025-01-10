+++
date = '2024-12-07T00:22:09+08:00'
draft = false
title = '第一篇Hugo文章'
+++


## 个人博客《红雨随心小站》的Github仓库

<div align="center">
  <table>
    <tr>
      <td style="vertical-align: middle;">
        <a href="//molimi20.github.io" target="_blank">
          <img src="https://github.com/molimi20/molimi20.github.io/blob/hugo/static/imgs/CuoTou.jpg?raw=true" alt="头像" style="width: 100px; height: 100px; border-radius: 50%;">
        </a>
      </td>
      <td style="vertical-align: middle;">
        <a href="//molimi20.github.io" target="_blank" style="text-decoration: none; color: inherit;">
          <h1 style="margin: 0;">红雨随心小站</h1>
        </a>
      </td>
    </tr>
  </table>
</div>

<div align="right">
  <p>请到我的小号 <a href="//2061360308.github.io">2061360308.github.io</a> 浏览构建后的站点</p>
</div>

## 🚀使用方法
<br>

> 此博客项目支持在Github云端完成编辑和发布一系列操作，只需浏览器即可无需配置本地环境
> 已配置Github Workflow负责在云端进行自动化构建以及自动部署到Github Pages

<br>

✍️编辑文章：访问[github.com/2061360308/2061360308.github.io](https://github.com/2061360308/2061360308.github.io) 仓库直接在线添加货编辑Markdown文件即可<br>

🖼️图床管理：博客使用腾讯云COS储存图片资源，点击使用[COSBrowser-Web](https://cosbrowser.cloud.tencent.com/web/file?bucket=blog-image-1303709080&region=ap-chengdu)工具在线管理

⚙️网站配置：可以编辑[`config.yaml`](//github.com/2061360308/2061360308.github.io/edit/hugo/config.yaml)<br>

🎨主题更改：直接修改[`.gitmodlues`](//github.com/2061360308/2061360308.github.io/edit/hugo/.gitmodlues)文件来更改子项目配置<br>

🔗友链编辑：点击修改[`flinks.yaml`](//github.com/2061360308/2061360308.github.io/deit/hugo/data/flinks.yaml)文件来管理友情链接<br>

🌐Github Dev：可以使用github.dev体验更完整的云IDE环境（速度较慢）[main分支](//github.dev/2061360308/2061360308.github.io/tree/main)、[hugo分支](//github.dev/2061306030/2061360308.github.io/tree/hugo)<br>

友链格式参考
```yaml
- name: NexT 主题
  desc: 保持简单的易用性和强大的功能。 # 支持HTML代码
  avatar: https://hugo-next.eu.org/imgs/hugo_next_avatar.png
  link: https://hugo-next.eu.org
```

## 🛠️构建说明

> 【分支】
> **hugo**分支下保存的是hugo创建的网站文件以及选用的主题Hugo NexT文件
> **main**分支下仅仅保存文章文件

项目已经配置了Workflow用来一键自动部署到Github Pages流程如下：
 - 会自动先检出hugo分支
 - 之后将main分支下的文章检出到./content/post文件夹下
 - 构建hugo网站
 - 发布到Github Page

**注意**：hugo分支的更改提交默认不会触发Github Pages的更新，需要手动激活Workflow

## 💻本地使用
此项目在云端即可运行，如果需要克隆到本地测试请按照下面步骤进行

1. 安装配置Hugo
2. 克隆项目的hugo分支
3. 克隆 main 分支到 content/posts 目录
4. 更新子模块

**Linux下命令示例**
```shell
# 克隆 hugo 分支
git clone -b hugo https://github.com/2061360308/2061360308.github.io.git
cd 2061360308.github.io

# 删除 content/posts 目录（如果存在且不包含重要内容）
rm -rf content/posts

# 克隆 main 分支到 content/posts 目录
git worktree add content/posts main

# 更新子模块（如果有）
git submodule update --init --recursive
```

**Windows Powershell下命令示例**
```shell
# 克隆 hugo 分支
git clone -b hugo https://github.com/2061360308/2061360308.github.io.git
cd 2061360308.github.io

# 删除 content/posts 目录（如果存在且不包含重要内容）
rmdir /S /Q content\posts

# 克隆 main 分支到 content/posts 目录
git worktree add content/posts main

# 更新子模块（如果有）
git submodule update --init --recursive
```

## 🔗相关链接
[Hugo](https://gohugo.io)

[Hugo中文文档](https://hugo.opendocs.io/)

[Hugo NexT演示站](https://hugo-next.eu.org/)

[Hugo NexT Github](https://github.com/hugo-next/hugo-theme-next/)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTY5NzMxNjg0NV19
-->
