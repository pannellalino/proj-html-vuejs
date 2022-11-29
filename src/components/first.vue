<script>
import cards from './data/cards';
import buttonCustom from './buttonCustom.vue';

export default {
  name: 'first',
  components:{
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
  <section>
    <div class="container text-center">
      <div class="row">
        <div class="offset-3 col-6">
          <h4 class="fw-bold mb-5">Let passion and determination be the guide along the way and develop at your own pace that's confortable.</h4>
          <h6 class="fw-bold">FANNIE MORENO</h6>
          <span class="text-secondary fw-light">/Founder & CEO</span>
        </div>
      </div>
      <div class="numbers my-5 py-4">
        <div class="mx-5" v-for="(num, index) in cards.numbers" :key="index">
          <h2 class="fw-bold">{{num.title}}</h2>
          <span class="text-secondary text-uppercase">{{num.descr}}</span>
        </div>
      </div>
      <div class="d-flex">
        <div class="container-cards cards py-5">
          <div class="d-flex flex-wrap pos justify-content-center">
            <div class="card me-4 my-4 text-start px-3 pt-3 border-0">
              <h5 class="fw-bold">Graphic Design</h5>
              <p class="text-secondary">Have a passion for graphic and arts? Show your talents with confidence and self-assertiveness.</p>
              <img src="../assets/img/home-6-service-image-01.png" alt="">
            </div>
            <div class="card me-4 my-4 text-start px-3 pt-3 border-0 move">
              <h5 class="fw-bold">Business Administration</h5>
              <p class="text-secondary">Learners are encouraged to study the mechanism and structure of system administration.</p>
              <div class="image text-center">
                <img class="h-100" src="../assets/img/home-6-service-image-02.png" alt="">
              </div>
            </div>
            <div class="card me-4 my-4 text-start pe-3 pt-3 border-0">
              <div class="image text-start">
                <img class="h-100" src="../assets/img/home-6-service-image-03.png" alt="">
              </div>
              <h5 class="fw-bold ps-3">Idea Discussion</h5>
              <p class="text-secondary ps-3">Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
            </div>
            <div class="card me-4 my-4 text-start px-3 pt-3 border-0 move">
              <div class="image text-center">
                <img class="w-100" src="../assets/img/home-6-service-image-04.png" alt="">
              </div>
              <h5 class="fw-bold">Web Development</h5>
              <p class="text-secondary">Learn to start building a webpage from scratch. You decide your own pace, course and speed.</p>
            </div>       
          </div> 
        </div>
        <div class="text col-4 text-start pe-4">
          <h6 class="text-uppercase text-secondary">Together we can create</h6>
          <h2 class="fw-bold my-2">Services We <span class="fw-light text-success">Can Provide</span> For My Clients.</h2>
          <ul v-for="(list, index) in cards.lista" :key="index">
            <li class="text-secondary my-2"><i class="fa-solid fa-check me-2"></i>{{list}}</li>
          </ul>
          <buttonCustom class="btn w-50 ms-0"/>
        </div>
      </div>
    </div>
  </section>
</template>  

<style lang="scss" scoped>
.container{
  background-image: url('../assets/img/background-pattern-grid-line.png');
  padding-top: 150px;
  .cards{
    width: 50%;
    position: relative;
  }
  .card{
    width: calc(100% / 3);
    box-shadow: 0px 1px 20px 1px lightgray;
    &:hover{
      box-shadow: none;
    }
    .image{
      height: 142px;
      width: 100%;
    }
  }
  .move{
    position: relative;
    bottom: -20px;
  }
  .text{
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .fa-check{
    color: #27ab94;
  }
  .btn{
    &:hover{
      color: white;
      background-color: #293259;
    }
  }
  .numbers{
    display: flex;
    justify-content: center;
    h2{
      color: #27ab94;
    }
    span{
      font-size: .8rem;
    }
  }
}
</style>