---
layout: cover
---
# 01 MarkDoc
<div class="flex justify-center">
<p class="w-71 text-center text-zinc-300">MarkDoc 是 Markdown 的超集,通过它可扩展 Markdown 语法</p>
</div>

---
layout:cover
---
# 01 MarkDoc 

[官网](https://markdoc.dev/)

<div grid="~ cols-2 gap-4">

<div class="h-85 flex justify-center items-center">

<div v-if="$slidev.nav.clicks === 0" class="w-96 text-center">
<p>
MarkDoc 是 Markdown 的超集。它扩展了 Markdown 语法并且它可以自定义组件进行渲染。极大地提高了 Markdown 的灵活性。
</p>
<p>
<icon-park-solid-bad-two class="mr-4"/>缺点：它官方并没有提供 Vue 的渲染器需要我们根据 transform 出来的结果去实现。我们可以通过安装一些库来实现渲染 Vue 组件<br/>(比如: vue-markdoc)
</p>
</div>
<div v-if="$slidev.nav.clicks === 1">
MarkDoc 源码
</div>
<div v-if="$slidev.nav.clicks === 2">
把 MarkDoc 源码解析形成 AST
</div>
<div v-if="$slidev.nav.clicks === 3">
把 AST 转化 为可渲染的树结构
</div>
<div v-if="$slidev.nav.clicks === 4" class="text-center">
调用 HTML 渲染函数，渲染出 DOM
<p class="text-center">
(注意:MarkDoc 官方并没有提供 Vue 的渲染器)
</p>
</div>
</div>
<div class="flex justify-center flex-col h-85">

```js
npm install @markdoc/markdoc
```

```js{all|3-6|7|8|9}
import Markdoc from '@markdoc/markdoc';

const doc = `
# Hello world.
> My first Markdoc page
`;
const ast = Markdoc.parse(doc);
const content = Markdoc.transform(ast);
const html = Markdoc.renderers.html(content);
```
</div>

</div>