# docsify 文档模板

```md
|-- docsify-template
    |-- .gitignore
    |-- README.md // 做为主页内容渲染
    |-- docs
        |-- .nojekyll // 用于阻止 GitHub Pages 会忽略掉下划线开头的文件
        |-- index.html // 入口文件
        |-- quick-start.md
        |-- README.md
        |-- _coverpage.md // 封面
        |-- _navbar.md // 导航栏
        |-- _sidebar.md // 侧边栏
        |-- images
        |   |-- process.png
        |-- media
            |-- favicon.ico
            |-- _favicon.ico
```

## 快速开始

安装 docsify-cli 工具，可以方便创建及本地预览文档网站。

```bash
npm i docsify-cli -g
```

## 初始化项目
如果想在项目的 ./docs 目录里写文档，直接通过 init 初始化项目。

```bash
docsify init ./docs

# or
git clone https://github.com/Mrlhz/docsify-template
cd docsify-template
docsify serve docs
```

## 本地预览网站

本地实时预览，默认访问 http://localhost:3000 。

```bash
docsify serve docs
# or 端口号默认3000
docsify serve docs -p 3000
```
