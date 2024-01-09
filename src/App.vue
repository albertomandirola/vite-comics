<script>
import AppHeader from "./components/AppHeader.vue"
import AppMain from "./components/AppMain.vue"
import AppFooter from "./components/AppFooter.vue"
import BlueBar from "./components/BlueBar.Vue"
export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    BlueBar
  }
}
</script>
<template lang="">
  <div>
    <AppHeader />
    <AppMain />
    <BlueBar />
    <AppFooter />
  </div>
</template>
<style lang="scss">
@use './styles/generals.scss' as *;
</style>