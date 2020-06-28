<template>
  <div id="app">
    <Home />
  </div>
</template>

<script>
import Home from '@/components/home/HomePage'
export default {
  name: 'App',
  components: {
    Home,
  },
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}
body {
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Montserrat', sans-serif;
  font-size: 18px;
}
</style>
