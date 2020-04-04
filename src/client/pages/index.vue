<template>
  <div class="index-wrapper">
    <div>
      <div class="container index-content">
        <p>我们是一个严肃的，有8年历史的</p>
        <p>原版生存服务器</p>
        <p class="small-desc">（已更新到1.15.2惹！）</p>
        <button @click="nyan" class="btn-cat73">戳一下二喵屁股</button>
      </div>
      <div>
        <div>
          <div></div>
        </div>
      </div>
    </div>
    <video
      autoplay
      loop
      muted
      class="background-video"
      src="/videos/Buzzy Bees- Official Trailer.mp4"
    ></video>
  </div>
</template>

<script>
export default {
  methods: {
    nyan() {
      this.$message.info('奇怪的数字增加惹~')
    }
  }
}
</script>
<style lang="less">
.index-wrapper {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.index-content {
  margin: 0 auto;
  color: white;
  font-size: 46px;
  line-height: 62px;
  text-align: center;
  font-weight: 600;
  .small-desc {
    font-size: 18px;
    line-height: 40px;
    font-weight: 400;
  }
}
.background-video {
  position: fixed;
  right: 0;
  bottom: 0;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  height: auto;
  z-index: -100;
  background: url(/videos/video-poster.jpg) no-repeat;
  background-position: center;
  background-size: cover;
}
.btn-cat73 {
  font-size: 20px;
  width: 191px;
  height: 58px;
  background: rgba(252, 154, 27, 1);
  border-radius: 35px;
  border: none;
  color: white;
  font-weight: 600;
  cursor: pointer;
  transition: background-color 0.5s;

  &:hover {
    background: #ffbb65;
  }
}
</style>
