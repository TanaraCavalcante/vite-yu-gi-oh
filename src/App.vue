<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

export default {
  data() {
      return{

      }
  },
  components:{
    AppHeader,
    AppMain
  }
}
</script>

<template>
  <AppHeader/>
  <AppMain class="container"/>
</template>

<style lang="scss">
 @use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
 @use "./style/general.scss" as *;
// @use "./style/partials/variables.scss" as *;
</style>
