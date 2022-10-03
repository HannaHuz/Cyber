<template>
  <section class="goods">
    <vue-tiny-slider class="goods-slider" v-bind="tinySliderOptions">
      <img v-for="i in 3" :src="require(`@/assets/img/product-${i}.png`)">
    </vue-tiny-slider>
  </section>
</template>
<script>
export default{
  data(){
    return {
      tinySliderOptions: {
        mouseDrag: true,
        items: 1,
        swipeAngle: false,
        nav: true,
        loop: false,
        preventScrollOnTouch: 'auto'
      }
    }
  }
}
</script>
<style lang="scss">
.goods {
  .tns-outer {
    position: relative;
  }
  .tns-nav {
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translate(calc(-50% + 40px), 30px);
    height: 16px;
    display: flex;
    align-items: center;
    @media(min-width:768px){
      transform: translate(calc(-50% + 40px), 60px);
    }
    button {
      border: none;
      background: rgba(114, 94, 137, 0.5);
      width: 40px;
      height: 2px;
      @media(min-width:768px){
        width: 100px;
      }
    }
    &-active {
      background: #725E89!important;
    }
  }
  .tns-controls {
    display: flex;
    box-shadow: none;
    position: absolute;
    z-index: 10;
    bottom: 0;
    left: 50%;
    transform: translate(calc(-100% - 40px), 30px);
    @media(min-width:768px){
      transform: translate(calc(-250% - 40px), 60px);
    }
    &:focus, &:hover, &:active {
      -webkit-appearance: none;
    }
    button {
      width: 32px;
      height: 16px;
      padding: 0;
      background: none;
      border: none;
      outline: none;
      color: transparent;
      background: url('@/assets/img/arrow.svg') no-repeat center center/contain;
      transition: 0.5s ease;
      &:hover {
        opacity: 0.5;
      }
      &[data-controls="prev"]{
        transform: rotate(180deg);
      }
    }
  }
}
</style>