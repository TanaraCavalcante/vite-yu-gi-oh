<script>
import MainListItem from './MainListItem.vue';

  export default {
    data() {
        return{

        }
    },
    components:{
        MainListItem,
    }
}
</script>

<template>
    <section class="container">
      <h3>Main list</h3>
    </section>

    <MainListItem/>
</template>

<style lang="scss" scoped>
    section {
        background-color: white;
        margin-top: 10px;
        margin-left: 80px;
        
    }
</style>