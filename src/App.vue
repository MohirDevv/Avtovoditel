<template>
  <Header/>
  <TalimInfo/>
  <TextSection/>
  <PriceSection/>
  <ImageSection/>
</template>

<script>
import Header from './components/Header.vue';
import ImageSection from './components/ImageSection.vue';
import PriceSection from './components/PriceSection.vue';
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
    TextSection,
    PriceSection,
    ImageSection
}
}
</script>