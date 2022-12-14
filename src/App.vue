<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import JumboTron from './components/JumboTron.vue';

export default {
  // name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppMain,
    JumboTron
  }
}
</script>

<template>


  <AppHeader/>

  <JumboTron/>
  
  <main>

  <AppMain/>

  </main>

  <AppFooter/>
</template>

<style lang="scss">

@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;


</style>
