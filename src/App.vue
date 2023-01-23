<template>
  <div id="app">
    <MyHeader></MyHeader>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
  }
}
</script>

<style lang="scss">
@import "./assets/general.scss";
</style>
