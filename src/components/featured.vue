<script>
import AppCard from './AppCard.vue';
import buttonCustom from './buttonCustom.vue';
import cards from './data/cards';


export default {
  name: 'featured',
  components:{
    AppCard,
    buttonCustom
  },
  data(){
    return{
      cards
    }
  }
}
</script>

<template>
  <section class="text-center p-5">
    <div class="container text-center">
      <h6>Choose a course to get started</h6>
      <h2 class="p-2"><strong class="text-dark fw-bold">Latest Featured </strong>Courses</h2>
    </div>
    <div class="container d-flex flex-wrap py-5">
      <AppCard 
      v-for="(card, index) in cards.courses"
      :key="index"
      :card="card"
      />
    </div>
    <buttonCustom />
  </section>
</template>  

<style lang="scss" scoped>
section{
  background-color: #f6f3f6;
  h6{
    text-transform: uppercase;
    color: grey;
  }
  h2:not(strong){
    color: #27ab94;
    font-weight: 100;
  }
}
</style>