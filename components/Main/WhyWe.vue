<template>
  <section class="whywe">
    <div class="container">
      <h2>Почему мы</h2>
      <vue-tiny-slider v-bind="tinySliderOptions">
        <div class="whywe-item" v-for="(slide, i) in slides" >
          <div class="whywe-left">
            <h3 v-html="slide.title"></h3>
            <p v-html="slide.text"></p>
          </div>
          <div class="whywe-right">
            <img :src="require(`@/assets/img/whywe-${++i}.png`)">
          </div>
        </div>
      </vue-tiny-slider>
    </div>
  </section>
</template>
<script>
export default{
  data(){
    return {
      slides: [
        {
          title: 'Налаженный контакт с дистрибьюторами ',
          text: 'Мы лично посещаем наших дистрибьюторов в Китае, для контроля качества каждого товара, материала и техники для того, чтобы Вы были уверенны в используемом оборудовании, которое поставляет команда <b>CyberLink</b>'
        },
        {
          title: 'Налаженный контакт с дистрибьюторами ',
          text: 'Мы лично посещаем наших дистрибьюторов в Китае, для контроля качества каждого товара, материала и техники для того, чтобы Вы были уверенны в используемом оборудовании, которое поставляет команда <b>CyberLink</b>'
        },
        {
          title: 'Налаженный контакт с дистрибьюторами ',
          text: 'Мы лично посещаем наших дистрибьюторов в Китае, для контроля качества каждого товара, материала и техники для того, чтобы Вы были уверенны в используемом оборудовании, которое поставляет команда <b>CyberLink</b>'
        },
      ],
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
.whywe {
  .tns-outer {
    position: relative;
  }
  .tns-nav {
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translate(calc(-50% + 40px), 40px);
    height: 16px;
    display: flex;
    align-items: center;
    @media(min-width: 992px){
      left: 0;
      transform: translate(+104px, 0);
    }
    button {
      border: none;
      background: rgba(114, 94, 137, 0.5);
      width: 40px;
      height: 2px;
      @media(min-width:992px){
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
    transform: translate(calc(-100% - 40px), 40px);
    @media(min-width: 992px){
      transform: translate(0,0);
      left: 0;
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
<style lang="scss" scoped>
.whywe{
  padding: 80px 0;
  @media(min-width:768px){
    padding-top: 160px;
    padding-bottom: 110px;
  }
  .container {
    max-width: 1173px;
  }
  h2 {
    font-weight: 700;
    font-size: 22px;
    line-height: 1.3;
    text-transform: uppercase;
    color: #2A0E49;
    margin-bottom: 40px;
    @media(min-width:992px){
      font-size: 32px;
      line-height: 44px;
      margin-bottom: 60px;
    }
  }
  &-item{
    display: inline-flex!important;
    align-items: flex-start;
    justify-content: space-between;
  }
  &-left {
    width: 50%;
    @media(min-width:768px){
      width: 44.3%;
      width: calc(50% - 30px);
      position: relative;
      display: inline-block;
    }
  }
  &-right {
    width: 45%;
    @media(min-width:768px){
      display: inline-block;
      width: 35.3%;
      margin-left: 20.48%;
    }
  }
  h3 {
    font-weight: 700;
    font-size: 15px;
    line-height: 1;
    color: #2A0E49;
    margin-bottom: 20px;
    @media(min-width:768px){
      font-size: 24px;
      line-height: 33px;
      margin-bottom: 40px;
    }
  }
  p {
    font-weight: 400;
    font-size: 14px;
    line-height: 1;
    color: #2A0E49;
    @media(min-width:768px){
      font-size: 18px;
      line-height: 25px;
    }
  }
}
</style>