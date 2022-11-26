<script>
import buttonCustom from './buttonCustom.vue';

export default {
  name: 'jumbotron',
  components:{
    buttonCustom

  }

}
</script>

<template>
  <div class="jumbo text-center pt-4">
    <h1 class="text-center text-white pt-4 fw-bolder">Learn At Your Own Pace!</h1>
    <h6 class="text-center text-white-50">Get teamed up with people of the same will.</h6>
    <buttonCustom /><br>

    <div class="container-c m-0">
      <div class="row w-100 mt-5 justify-content-center">
        <div class="col-2 d-flex justify-content-center">
          <img class="h-100" src="../assets/img/home-6-hero-left-person.png" alt="">
        </div>
        <div class="col-5 p-0">
          <img class="image-center w-100" src="../assets/img/home-6-hero-poster-final.jpg" alt="jumbo">
        </div>
        <div class="image-right col-2 p-0  d-flex flex-column justify-content-end">
          <img src="../assets/img/home-6-hero-right-person.png" alt="">
        </div>
      </div>
    </div>

  </div>
</template>  

<style lang="scss" scoped>
.jumbo{
  position: relative;
  width: 100%;
  background-image: url('../assets/img/wave5.svg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: left;
  background-color: #293259;
  .container-c{
    position: relative;
    bottom: -70px;
    .image-center{
      border: 25px solid white;
      border-radius: 25px;
      box-shadow: 2px 1px 50px 0px  rgba(35, 35, 35, 0.616);
    }
    .image-right{
      width: 250px;
    }
  }
}
</style>