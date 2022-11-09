<script>
import AppHeader from "./components/AppHeader.vue"
import ContentSection from "./components/ContentSection.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
export default{
  components:{
    AppHeader,
    ContentSection,
    AppMain,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <ContentSection />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as*;
</style>