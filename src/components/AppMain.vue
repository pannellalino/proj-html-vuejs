<script>
import jumbotron from './jumbotron.vue';
import first from './first.vue';
import featured from './featured.vue';

export default {
  name: 'AppMain',
  components:{
    jumbotron,
    first,
    featured
  },
  data(){
    return{
    }
  }

}
</script>

<template>
  <main>
    <jumbotron />
    <first />
    <featured />
  </main>
</template>  

<style lang="scss" scoped>

</style>