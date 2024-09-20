<script>
  export default {
    data() {
        return{

        }
    }
}
</script>

<template>
    <section class="container" id="card">
      <div class="card" style="width: 70px;" v-for="(item,i) in 20" :key="i">
        <img src="..." class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title"> {{ item }}</h5>
            <p class="card-text">descricao</p>
        </div>
     </div>
    </section>
</template>

<style lang="scss" scoped>
    

</style>