<template>
  <div class="full-layout">
    <side-nav></side-nav>
    <nuxt class="full-body" />
  </div>
</template>
<script>
import SideNav from '~/components/SideNav.vue'

export default {
  components: {
    SideNav
  }
}
</script>
<style lang="less">
body,
#__nuxt,
#__layout,
.full-layout {
  height: 100vh;
}

.full-layout {
  display: flex;
  flex-direction: column;

  .full-body {
    flex-grow: 1;
    flex-shrink: 1;
  }
}
</style>
