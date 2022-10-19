---
layout: cover
---
# 03 Yeoman
<div class="flex justify-center">
<p class="w-80 text-center text-zinc-300">Yeoman 向我们提供便捷的脚手架服务</p>
</div>

---
layout:cover
---
# 03 Yeoman

[官网](https://yeoman.io/)

<div grid="~ cols-2 gap-4">

<div class="h-85 flex justify-center items-center">

<div v-if="$slidev.nav.clicks === 0" class="w-96 text-c">
<p>
情景:如果现在有个项目现在需要开始开发,你需要搭建一个框架出来给大家使用,你会怎么做？<br/>
<br/>大部分人做法:我们一般首先用 Vite 等脚手架工具生成一个项目然后再开发。
<br/><br/>
这样做有什么不好？
<br/><br/>
假如你开发的是 Vue 项目,用了 Vite 生成了一个工程,你还是要安装并配置诸如 vuex , axios , vue-router 等等的库。这个就有点麻烦了,为什么我们不开发一个项目生成器帮助我更快完成任务呢？而Yeoman 就是
用来快速开发运行私人的代码生成器的一个工具。
</p>

</div>
</div>
<div class="flex justify-center flex-col h-85">

```js
# 安装
npm install -g yo
```

![yeoman](/img/yo.png)
</div>

</div>