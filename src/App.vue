<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppMidNav from './components/AppMidNav.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  components: {
    AppHeader,
    AppMain,
    AppMidNav,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppMidNav />
  <AppFooter />
</template>

<style scoped></style>
