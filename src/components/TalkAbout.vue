<script>
import cards from './data/cards';

export default {
  name: 'TalkAbout',
  data(){
    return{
      cards
    }
  }
}
</script>

<template>
  <div class="container text-center">
    <h2 class="pt-5"><strong class="text-dark fw-bold">Why People Talk About </strong>MaxCoach<span class="text-dark fw-bold">?</span></h2>
    <div class="testimonial d-flex align-items-center p-5">
      <div class="image">
        <div class="image-2">
          <img class="pic m-5 rounded-circle" src="../assets/img/testimonial-avata-02.jpg" alt="">
        </div>
      </div>
      <p class="px-5 fs-3 fw-light text-start">I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.<br><span class="fw-bold fs-6 text-uppercase">Mina Hollace<br></span><span class="text-secondary fs-6">/Freelancer</span></p>
    </div>
    <div class="logos align-items-center pb-5">
      <div v-for="(logo, index) in cards.logos"
        :key="index">
        <img class="p-5"
        :src="'../src/assets/img/' + logo.logo" alt="">
      </div>
    </div>
  </div>
</template>  

<style lang="scss" scoped>
h2{
  color: #27ab94;
  font-weight: 100;
}
.pic{
  width: 150px;
  height: 150px;
  object-fit: cover;
}
.logos{
  display: flex;
  justify-content: center;
}
.image{
  background-image: url('../assets/img/maxcoach-shape-05-150x150.png');
  background-repeat: no-repeat;
  background-size: 100px;
  background-position: 100px 140px;
}
.image-2{
  background-image: url('');
}

</style>