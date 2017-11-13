<template>
    <div id="app">
        <app-header></app-header>

        <router-view></router-view>
    </div>
</template>

<script>
import appHeader from '@/components/common/appHeader'

export default {
  name: 'app',
  components: {
    'app-header': appHeader
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
