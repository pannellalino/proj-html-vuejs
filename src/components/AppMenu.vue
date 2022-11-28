<script>
export default {
  name: 'AppMenu'

}
</script>

<template>

  <ul class="w-100 justify-content-end d-flex">
    <li class="me-4">
      <select class="border-0 p-0 bg-transparent text-white" name="" id="">
        <option value="Home">Home</option>
      </select>
    </li>
    <li class="me-4">
      <select class="border-0 p-0 bg-transparent text-white" name="" id="">
        <option value="Home">Pages</option>
      </select>
    </li>
    <li class="me-4">
      <select class="border-0 p-0 bg-transparent text-white" name="" id="">
        <option value="Home">Courses</option>
      </select>
    </li>
    <li class="me-4">
      <select class="border-0 p-0 bg-transparent text-white" name="" id="">
        <option value="Home">Features</option>
      </select>
    </li>
    <li class="me-4">
      <select class="border-0 p-0 bg-transparent text-white" name="" id="">
        <option value="Home">Blog</option>
      </select>
    </li>
    <li class="">
      <select class="border-0 p-0 bg-transparent text-white" name="" id="">
        <option value="Home">Shop</option>
      </select>
    </li>
    <li class="me-4">
      <i class="bi bi-cart3 text-white position-relative">
        <span class="position-absolute top-0 start-100 translate-middle badge rounded-circle bg-white">0
        </span>
      </i>
    </li>
    <li class="user-c me-4">
      <i class="fa-regular fa fa-circle-user text-white"></i>
    </li>
  </ul>

</template>  

<style lang="scss" scoped>

.bi-cart3{
  font-size: 18px;
}
.badge{
  padding-left: 3.5px;
  padding-right: 6.5px;
  padding-top: 2px;
  padding-bottom: 2px;
  color: black;
}
.user-c{
  margin: auto 0;
  font-size: 18px;
}

</style>