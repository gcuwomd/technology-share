---
layout: cover
---
# 02 Tldr
<div class="flex justify-center">
<p class="w-71 text-center text-zinc-300">Tldr 是命令行小抄工具,帮助你查询一些命令的用法</p>
</div>

---
layout:cover
---
# Tldr

[官网](https://tldr.sh/)

<div grid="~ cols-2 gap-4">

<div class="h-85 flex justify-center items-center">

<div v-if="$slidev.nav.clicks === 0" class="w-96 text-right">
<p>
你是否有过在 Linux 环境下想用某个命令,<br />但是这个命令你又不太熟悉它的用法的经历？
</p>
<p>而 Tldr 就是为了解决这情况而生的,它会用最简单的例子教会你如何使用这个命令。<br/>
比如:你不会 tar 命令的用法<br/>键入：
<span >

```js
npm install -g tldr
tldr tar
```
</span>即可查询到 tar 命令用法
</p>


</div>
</div>
<div class="flex justify-center flex-col h-85">

![tldr演示](img/tldr.gif)
</div>

</div>