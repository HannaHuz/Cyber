<template>
  <div class="page page-main">
    <Preloader v-if="preloader" />
    <Header v-if="loaded" />
    <MainBanner v-if="loaded" />
    <MainService v-if="loaded" />
    <MainWhyWe v-if="loaded" />
    <MainDealwith v-if="loaded"/>
    <MainGoodsCarousel v-if="loaded" />
    <MainCatalog v-if="loaded" />
    <MainBrands v-if="loaded"/>
    <ContactUs v-if="loaded" />
    <Footer v-if="loaded" />
    <Copyrights v-if="loaded" />
  </div>
</template>
<script>
export default {
  layout:'default',
  head() {
    return {
      title: 'CyberLink | Главная страница'
    }
  },
  data(){
    return {
      loaded: false,
      preloader: true
    }
  },
  mounted(){
    setTimeout(()=>{
      this.loaded = true
      if(this.loaded){
        this.preloader = false
      }
    }, 2000);
  }
}
</script>
