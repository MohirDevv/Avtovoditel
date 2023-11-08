<template>
  <Header/>
  <TalimInfo/>
  <TextSection/>
</template>

<script>
import Header from './components/Header.vue';
import TalimInfo from './components/TalimInfo.vue';
import TextSection from './components/TextSection.vue';


export default {
  data(){
    return{   
    }
  },
  components: {
    Header,
    TalimInfo,
    TextSection
}
}
</script>