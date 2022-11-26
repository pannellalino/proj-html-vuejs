<script>
import cards from './data/cards';

export default {
  name: 'Blogs',
  data(){
    return{
      cards
    }
  }

}
</script>

<template>
  <section class="p-5">
    <div class="container text-center">
      <h6 class="text-secondary text-uppercase">Enjoy readingon maxcoach</h6>
      <h2 class="p-2"><strong class="text-dark fw-bold">Latest on </strong>Our Blogs</h2>
    </div>
    <div class="container d-flex">
      <article v-for="(artic, index) in cards.articolis"
      :key="index" class="p-4">
        <img class="mb-4 rounded" :src="'../src/assets/img/' + artic.file_name" alt="">
        <span class="text-secondary text-uppercase">{{artic.job}}</span>
        <h5 class="fw-bold mt-2">{{artic.info}}</h5>
        <span class="pe-4 text-secondary"><i class="fa-regular fa-calendar me-2"></i>{{artic.date}}</span>
        <span class="text-secondary"><i class="fa-solid fa-eye me-2"></i>{{artic.views}}</span>
      </article>
    </div>
  </section>
</template>  

<style lang="scss" scoped>
section{
  background-color: #f6f3f6;
}
h2{
  color: #27ab94;
  font-weight: 100;
}
article{
  width: calc(100% / 3);
  img{
    width: 100%;
    object-fit: cover;
  }
  span{
    font-size: 14px;
  }
}
</style>