<script>
import MainList from './MainList.vue';

  export default {
    data() {
        return{

        }
    },
    components:{
        MainList,
    }
}
</script>

<template>
    <div class="container">
    <input type="text">
    </div>

    <MainList/>
    
</template>

<style scoped>

   div{
    margin-top: 10px;
   }
 
</style>