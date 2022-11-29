<script>
export default {
  name: 'HelpYou'

}
</script>

<template>
  <section class="p-5">
    <div class="container text-center mb-5">
      <h6 class="text-uppercase">Wanna transform your life?</h6>
      <h2 class="fw-bold p-2">Glad to <span>Help You</span> Learn</h2>
    </div>
    <div class="container">
      <article class="d-flex">
        <div class="card bg-transparent border-0">
          <i class="fa-regular fa-flag mb-4 fs-1"></i>
          <h6 class="fw-bold">Idea Discussion</h6>
          <p class="text-secondary fw-light">Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
        </div>
        <div class="card bg-transparent border-0">
          <i class="fa-solid fa-gear mb-4 fs-1"></i>
          <h6 class="fw-bold">Web Development</h6>
          <p class="text-secondary fw-light">Learn to start building a webpage from scratch. You decide your own pace, course and speed.</p>
        </div>
        <div class="card bg-transparent border-0">
          <i class="fa-regular fa-circle mb-4 fs-1"></i>
          <h6 class="fw-bold">System Administration</h6>
          <p class="text-secondary fw-light">Learners are encouraged to study the mechanism and structure of system administration.</p>
        </div>
        <div class="card bg-transparent border-0">
          <i class="fa-solid fa-desktop mb-4 fs-1"></i>
          <h6 class="fw-bold">Graphic Design</h6>
          <p class="text-secondary fw-light">Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.</p>
        </div>
      </article>
    </div>
    <div class="image text-center">
      <img src="../assets/img/home-6-services-image-768x308.png" alt="">
    </div>
  </section>
</template>  

<style lang="scss" scoped>
section{
  background-color: rgb(230, 230, 230);
}
span{
  font-weight: 100;
  color: #27ab94;
}
img{
  position: relative;
  bottom: -69px;
}
article{
  .card{
    width: calc(100% / 4);
    padding: 10px 30px 10px 10px
  }
}
</style>