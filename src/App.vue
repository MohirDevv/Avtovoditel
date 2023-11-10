<template>
  <Header />
  <TalimInfo />
  <TextSection />
  <PriceSection />
  <ImageSection />
  <MapSection />
  <SertificateSection />
</template>

<script>
import Header from "./components/Header.vue";
import ImageSection from "./components/ImageSection.vue";
import MapSection from "./components/MapSection.vue";
import PriceSection from "./components/PriceSection.vue";
import SertificateSection from "./components/SertificateSection.vue";
import TalimInfo from "./components/TalimInfo.vue";
import TextSection from "./components/TextSection.vue";

export default {
  data() {
    return {};
  },
  components: {
    Header,
    TalimInfo,
    TextSection,
    PriceSection,
    ImageSection,
    MapSection,
    SertificateSection,
  },
};
</script>

<style>
::-webkit-scrollbar {
  width: 12px; /* Ширина скроллбара */
}

::-webkit-scrollbar-thumb {
  background-color: #a0a0a0; /* Цвет ползунка */
  border-radius: 2px; /* Скругление углов ползунка */
}

::-webkit-scrollbar-track {
  background-color: #f0f0f0; /* Цвет фона дорожки */
  border-radius: 1px; /* Скругление углов дорожки */
}
</style>
