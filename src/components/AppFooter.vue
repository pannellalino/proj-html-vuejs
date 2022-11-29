<script>
export default {
  name: 'AppFooter'

}
</script>

<template>
  <footer class="text-center p-5">
    <div class="container pb-5">
      <div class="row">
        <div class="offset-1 col-3">
          <ul class="text-start">
            <li><strong class="text-dark">Address</strong></li>
            <li>382 NE 191st # 87394 Miami, FL 33179-3899</li>
            <li>+1(305) 547-9909 (9am - 5pm EST,Monday -Friday)</li>
            <li>support@maxcoach.com</li>
          </ul>
        </div>
        <div class="offset-1 col-2">
          <ul class="text-start">
            <li><strong class="text-dark">Explore</strong></li>
            <li>Start here</li>
            <li>Blog</li>
            <li>About us</li>
          </ul>
        </div>
        <div class="col-2">
          <ul class="text-start">
            <li>&nbsp</li>
            <li>Success story</li>
            <li>Courses</li>
            <li>Contact us</li>
          </ul>
        </div>
        <div class="col-2">
          <ul class="text-start">
            <li><strong class="text-dark">Information</strong></li>
            <li>Membership</li>
            <li>Purchase guide</li>
            <li>Privacy policy</li>
            <li>Terms of services</li>
          </ul>
        </div>
      </div>
      <div class="icons text-secondary offset-1 col-3 text-start">
        <i class="fa-brands fa-square-facebook"></i>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-instagram"></i>
        <i class="fa-brands fa-linkedin"></i>
      </div>
    </div>
    <span class="text-secondary">2020 Maxcoach. All Rights Reserved</span>
    <button class="rounded-circle"><a href="up"><i class="fa-solid fa-arrow-up"></i></a></button>
  </footer>
</template>  

<style lang="scss" scoped>
footer{
  background-color: #f6f3f6;
  position: relative;
  span{
    font-size: .8rem;
  }
  li:not(strong){
    color: grey;
  }
  button{
    border: 0;
    position: absolute;
    bottom: 20px;
    right: 20px;
    width: 50px;
    height: 50px;
    background-color: #27ab94;
    color: white;
    font-size: 20px;
    &:hover{
      background-color: #293259;
    }
  }
  ul{
    li{
      font-size: .9rem;
      margin-bottom: 5px;
    }
  }
  .icons{
    i{
      margin-right: 30px;
    }
  }
}
</style>