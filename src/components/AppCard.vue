<script>
export default {
  name: 'AppCard',
  props:{
    card: Object
  }
}
</script>

<template>
      <div class="card d-flex flex-row align-items-center p-3">
        <div class="image pe-4">
          <img class="rounded-circle" :src="'../src/assets/img/' + card.file_name" alt="">
        </div>
        <div class="text text-start">
          <h5><strong>{{card.price}}</strong></h5>
          <p v-html="card.info"></p>
          <span class="pe-4">{{card.lessons}}</span>
          <span>{{card.students}}</span>
        </div>
      </div>
</template>  

<style lang="scss" scoped>
.card{
  width: calc(100% / 2);
  border: 0;
  background-color: transparent;
    img{
      object-fit: cover;
      width: 170px;
      height: 170px;
    }
    h5{
      color: #27ab94;
    }
  }
</style>