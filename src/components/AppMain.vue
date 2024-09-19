<script>
import MainList from './MainList.vue';
import axios from "axios";

  export default {
    data() {
        return{
            cardList: [],
        }
    },
    components:{
        MainList,
    },
    methods:{
        getCardList(){
            axios.get('/user?ID=12345')
            .then(function (response) {
             // handle success
             console.log(response);
            })
            .catch(function (error) {
             // handle error
             console.log(error);
             })
            .finally(function () {
              // always executed
            });
         }
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