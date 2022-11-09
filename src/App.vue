<script>
import AppHeader from "./components/AppHeader.vue"
import ContentSection from "./components/ContentSection.vue";
import AppMain from "./components/AppMain.vue";
export default{
  components:{
    AppHeader,
    ContentSection,
    AppMain,
  }
}
</script>

<template>
  <AppHeader />
  <ContentSection />
  <AppMain />
</template>

<style lang="scss">
@use "./styles/general.scss" as*;
</style>