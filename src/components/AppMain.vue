<script>
import MainList from './MainList.vue';
import MainListItem from './MainListItem.vue';


  export default {
    data() {
        return{

        }
    },
    components:{
        MainList,
        MainListItem,
       
    }
}
</script>

<template>
    <div class="container">
    <input type="text">
    </div>

    <MainList/>
    <MainListItem/>
    
</template>

<style scoped>

   div{
    margin-top: 10px;
   }
 
</style>