<script>
import AppMenu from './AppMenu.vue';

export default {
  name: 'AppHeader',
  components:{
    AppMenu
  }

}
</script>

<template>
  <header>
    <div class="container d-flex align-items-center justify-content-between h-100">

      <img src="../img/light-logo.png" alt="logo">
      <AppMenu />
      <div class="input-group">
        <input type="text" class="form-control border-end-0" placeholder="Search..." aria-label="Recipient's username" aria-describedby="basic-addon2">
        <span class="input-group-text bg-white border-start-0" id="basic-addon2"><i class="fa-solid fa-magnifying-glass text-success"></i></span>
      </div>

    </div>
  </header>
</template>  

<style lang="scss" scoped>
header{
  width: 100%;
  height: 80px;
  background-color: #293259;
  img{
    height: 30px;
  }
  .input-group{
    width: 250px;
    ::placeholder{
      color: rgb(167, 166, 166);
      font-weight: 300;
    }
  }
}
</style>