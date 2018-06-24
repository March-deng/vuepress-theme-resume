## 🐈 介绍

当我们在使用 markdown 书写简历时，都有哪些痛点 🤒？

1.  使用编辑器自带的 markdown 预览。缺点：不够精致(丑)emmmm
2.  使用 Bear (付费)。缺点：导出 pdf 时无法修改参数(字体过大/过宽，导致页数增多)emmmm

于是...

![](imgs/eg.jpg)

## 🚀 开始

### 方式一：直接开始

1.  第一步：git clone 或 download 该项目

2.  第二步：

```bash
# 安装依赖包
yarn # 或 npm i

# 开始
yarn dev # 或 npm run dev
```

3.  第三步：修改 example/README.md

### 方式二：使用主题

```bash
yarn add -D vuepress-theme-resume # 或使用npm：npm i -D vuepress-theme-resume
```

```js
// .vuepress/config.js 中添加
theme: 'resume',
```

### 样式覆盖

创建 .vuepress/override.styl 文件

```css
/* font */
$fontSize = 13px
$fontWeight = 400

/* colors */
$accentColor = #4688F1
$textColor = #161F28
$borderColor = #eaecef
```

### 常见问题

> 如何导出为 pdf?

chrome 页面中右键 -> 打印 -> 另存为 pdf

> 导出的 pdf 如何控制只有 1 页？

方法一：.vuepress/override.styl 修改基准字体大小 $fontSize <br>
方法二：chrome 打印 -> 更多设置 -> 缩放

## 💡 协作

如果你有更好的想法，欢迎 PR 👏

如果它对你有所帮助，给我一个 star～ ⭐️
