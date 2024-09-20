<script>
import MainList from './MainList.vue';
import axios from "axios";

  export default {
    data() {
        return{
            cardList: [],
            apiUrl:"https://db.ygoprodeck.com/api/v7/cardinfo.php?num=25&offset=200",
        }
    },
    components:{
        MainList,
    },
    methods:{
        getCardList(){
            console.log("chiamata API iniziata");
            axios.get(this.apiUrl)
            .then((response) => {
             // handle success
             console.log(response.data.data);
             this.cardList = response.data.data;
            })
            .catch(function (error) {
             // handle error
             console.log(error);
             })
            .finally(function () {
              // always executed
              console.log('Chiamara api terminata!')
            });
         }
    },
    created(){
        this.getCardList()
    }
}
</script>

<template>
    
    <MainList :cards="cardList"/>
    
</template>

<style scoped>
 
</style>