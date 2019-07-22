# Headline

> An awesome project.

!> 一段重要的内容，可以和其他 **Markdown** 语法混用。

![logo](/media/Gakki.jpg ':size=160x160')

?> _TODO_ 完善示例

```bash
echo hello
```

<details>
<summary>代码示例</summary>

```js
let reg = /http: (\/\/.+.jpg)/;
let img1 = 'http: //img.hb.aicdn.com/bdad4f7788d7b3366c9f40406917848fa67bc7362bfa0-xLVh5p_fw658.jpg'
let img2 = '//img.hb.aicdn.com/4bfebd327513d3a20fbe51b591a763b8e901d776679ed-lPKjKd_fw658.jpg'
let str = img1.replace(reg, '$1')
console.log(str)
let date = '2018/10/30'
let pattern = /^(\d{4})[/-](\d{2})[/-](\d{2})$/
/*
  \d{4} 连续4个数字
  [/-]   / 或者 - 
  (\d{4}) 加个括号提取出来 用$1表示
*/
date.match(pattern) 
// ["2018/10/30", "2018", "10", "30", index: 0, input: "2018/10/30", groups: undefined]
RegExp.$1 // "2018"
let after = date.replace(pattern, '$1-$2-$3')
console.log(after)
```

</details>



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
            |-- b1725865767.ico
            |-- b935832691.ico
            |-- favicon.ico
            |-- favicon1.ico
            |-- Gakki-s.jpg
            |-- Gakki.jpg
            |-- _favicon.ico
```
