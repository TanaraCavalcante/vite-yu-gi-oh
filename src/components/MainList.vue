<script>
import MainListItem from './MainListItem.vue';

  export default {
    data() {
        return{

        }
    },
    components:{
        MainListItem,
    },
    props: {
        cards: {
            type: Array,
            required: true,
        }
    }
}
</script>

<template>
    <section class="container">
        <p >Found {{ cards.length }} cards!</p>
    </section>

    <MainListItem v-for="cardItem in cards" :key="cardItem.id" :card="cardItem" class="container"/>
</template>

<style lang="scss" scoped>
    section {
        margin-left: 20px;

        p{
            font-size: 12px;
            color: white;
            background-color: #212429;
            padding: 5px;
            margin-top: 10px;
            
        }
    }
</style>