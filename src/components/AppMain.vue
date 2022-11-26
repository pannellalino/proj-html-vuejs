<script>
import jumbotron from './jumbotron.vue';
import first from './first.vue';
import featured from './featured.vue';
import TalkAbout from './TalkAbout.vue';
import Blogs from './Blogs.vue';
import HelpYou from './HelpYou.vue';
import Certs from './Certs.vue';

export default {
  name: 'AppMain',
  components:{
    jumbotron,
    first,
    featured,
    TalkAbout,
    Blogs,
    HelpYou,
    Certs
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
    <Blogs />
    <HelpYou />
    <Certs />
  </main>
</template>  

<style lang="scss" scoped>

</style>