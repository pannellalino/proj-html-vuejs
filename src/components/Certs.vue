<script>
import buttonCustom from './buttonCustom.vue';


export default {
  name: 'Certs',
  components:{
    buttonCustom
  }

}
</script>

<template>
  <section class="p-5 text-center">
    <h5 class="pt-5 fw-bold">Start today for gettin <span class="fw-light">Online Certification</span></h5>
    <h3 class="fw-bold">You can be your own guiding star with our help!</h3>
    <buttonCustom class="button-c"/>
  </section>
</template>  

<style lang="scss" scoped>
section{
  span{
    color: #27ab94;
  }
  .button-c{
    &:hover{
      color: white;
      background-color: #293259;
    }
  }
}
</style>