<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppMain from "./components/AppMain.vue";
  import AppSlider from "./components/AppSlider.vue";
  import AppFooter from "./components/AppFooter.vue";
  import AppJumbotron from "./components/AppJumbotron.vue";

  export default {
  name: 'App',
  components:{
    AppHeader,
    AppMain,
    AppSlider,
    AppFooter,
    AppJumbotron,
    }
  }
</script>


<template>
  <AppHeader/>
  <AppJumbotron/>
  <AppMain/>
  <AppSlider/>
  <AppFooter/>
</template>


<style lang="scss">

@use './styles/general.scss';

</style>