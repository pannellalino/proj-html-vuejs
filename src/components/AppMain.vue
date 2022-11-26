<script>
import jumbotron from './jumbotron.vue';
import first from './first.vue';
import featured from './featured.vue';
import TalkAbout from './TalkAbout.vue';

export default {
  name: 'AppMain',
  components:{
    jumbotron,
    first,
    featured,
    TalkAbout
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
    <TalkAbout />
  </main>
</template>  

<style lang="scss" scoped>

</style>