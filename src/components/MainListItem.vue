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
   <section class="container">
    <div class="border">
        <img :src="card.card_images[0].image_url" alt="">
        <h3> {{ card.name }}</h3>
        <p>{{ card.race }}</p>
    </div>
  </section>
</template>

<style scoped>
  section{
    width: calc(100% / 4);
    background-color: white;
    padding-top: 5px;

    h3{
        font-size: 1.3rem;
        text-align: center;
    }

    p{
        text-align: center;
    }
  }
</style>