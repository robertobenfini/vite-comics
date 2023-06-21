<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppIcons from './components/AppIcons.vue';

export default {
  components:{
    AppHeader,
    AppMain,
    AppFooter,
    AppIcons
  }
}
</script>

<template>

  <div>

    <AppHeader />
    <AppMain />
    <AppIcons />
    <AppFooter />
    
  </div>

</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
  @use './styles/partials/variables' as *;
</style>