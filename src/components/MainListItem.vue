<script>
  export default {
    data() {
        return{

        }
    },
    props: {
        card:{
            type: Object,
            required: true,
        }
    }
}
</script>

<template>
   <section>
    <div>
        <img :src="card.card_images[0].image_url" alt="">
        <h3> {{ card.name }}</h3>
        <p>{{ card.race }}</p>
    </div>
  </section>
</template>

<style scoped>
  section{
    padding-top: 15px;
    width: 240px;
    height: 420px;
    display: inline-block;
    background-color: white;
    margin-bottom: 5px;
    

    div{
        display: flex;
        justify-content: center;
        flex-direction: column;
        


        h3{
        padding-top: 5px;
        font-size: 1rem;
        text-align: center;

        }

        p{
        text-align: center;
        font-size: 14px;
        }
    }
   
  }
</style>