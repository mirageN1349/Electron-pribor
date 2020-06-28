<template>
  <div class="main-wrap">
    <MainContent />
    <MainStock />
    <MainMenu />
  </div>
</template>

<script>
import MainContent from '@/components/home/MainContent'
import MainStock from '@/components/home/MainStock'
import MainMenu from '@/components/home/MainMenu'
export default {
  name: 'Home',

  components: {
    MainContent,
    MainStock,
    MainMenu,
  },
}
</script>

<style scoped lang="scss">
.main-wrap {
  display: flex;
  height: 100vh;
}
</style>
