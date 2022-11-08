<script>
import AppHeader from "./components/AppHeader.vue"
import ContentSection from "./components/ContentSection.vue";
export default{
  components:{
    AppHeader,
    ContentSection,
  }
}
</script>

<template>
  <AppHeader />
  <ContentSection />
</template>

<style lang="scss">
@use "./styles/general.scss" as*;
</style>