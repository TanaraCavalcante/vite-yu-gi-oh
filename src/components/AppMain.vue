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
        MainListItem
    }
}
</script>

<template>
   
    <div>
        <h1>Main</h1>
    </div>

    <MainList/>
    <MainListItem/>
</template>

<style scoped>
    h1{
        color: blue;
    }
 
</style>