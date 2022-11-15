<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppMain from "./components/AppMain.vue";
  import AppSlider from "./components/AppSlider.vue";
  import AppFooter from "./components/AppFooter.vue";

  export default {
  name: 'App',
  components:{
    AppHeader,
    AppMain,
    AppSlider,
    AppFooter
  }
  }
</script>


<template>
  <AppHeader/>
  <AppMain/>
  <AppSlider/>
  <AppFooter/>
</template>


<style lang="scss">

@use './styles/general.scss';

</style>