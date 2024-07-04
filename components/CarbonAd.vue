<template>
  <div ref="recommend" class="recommend">
    <a class="nicelinks" href="https://niceshare.site/?ref=cssfx.lovejade.cn">
      <img class="qrcode" src="https://niceshare.site/apple-touch-icon.png" alt="倾城之链" />
      <div class="desc">
        <div>
          <p class="title"><strong>逍遥自在轩</strong>，个人主页</p>
          <p>基于 Astro, Starlight, Svelte, Markdown, MDX，TailwindCSS, TypeScript 所构建的个人主页。</p>
        </div>
        <p>🏹 快速、易用、易于访问、高度可定制。</p>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  mounted() {
    this.$nextTick(() => { })
  }
}
</script>

<style>
.recommend {
  display: block;
  overflow: hidden;
  width: 520px;
  padding: 10px;
  margin: 0 auto;
  box-shadow: 0 1px 3px hsla(0, 0%, 0%, 0.05);
  border-radius: 4px;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell,
    'Helvetica Neue', Helvetica, Arial, sans-serif;
  line-height: 1.5;
  font-size: 12px;
  background-color: hsl(237, 37%, 24%);
  transform: scale(0.9);
}

.recommend .nicelinks {
  display: inline-block;
  height: 100px;
  color: inherit;
  text-decoration: none;
  display: flex;
}

.nicelinks .qrcode {
  width: 100px;
  height: 100px;
}

.nicelinks .desc {
  width: 400px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between;
  letter-spacing: 2px;
  padding-left: 15px;
}

.title {
  font-size: 14px;
}

@media screen and (max-width: 768px) {
  .recommend {
    width: 100%;
  }
}
</style>
