<template>
  <section class="catalog">
    <div class="container">
      <h2>каталог</h2>
      <ul class="catalog-list">
        <li v-for="item in catalogObj">
          <h3>{{item.name}}</h3>
          <img :src="item.img">
        </li>
      </ul>
    </div>
  </section>
</template>
<script>
  export default {
    data(){
      return{
        catalogObj: [
          {
            name: 'серверы',
            img: require('@/assets/img/catalog/catalog-1.png')
          },
          {
            name: 'Системы хранения данных',
            img: require('@/assets/img/catalog/catalog-2.png')
          },
          {
            name: 'Сетевое оборудование',
            img: require('@/assets/img/catalog/catalog-3.png')
          },
          {
            name: 'Компьютерная периферия',
            img: require('@/assets/img/catalog/catalog-4.png')
          }
        ]
      }
    }
  }
</script>
<style lang="scss" scoped>
.catalog {
  padding: 134px 0 30px;
  @media(min-width:992px){
    padding: 234px 0 30px;
  }
  h2 {
    font-weight: 700;
    font-size: 32px;
    line-height: 44px;
    text-transform: uppercase;
    color: #2A0E49;
    margin-bottom: 60px;
  }
  &-list {
    margin-bottom: 60px;
    @media(min-width:768px){
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      grid-auto-flow: row;
      gap: 20px;
    }
    li {
      cursor: pointer;
      position: relative;
      margin-bottom: 20px;
      transition: 0.5s ease;
      &:last-child {
        margin-bottom: 0;
      }
      @media(min-width:768px){
        margin-bottom: 0;
        &:nth-child(3){
          grid-column: 3/4;
          grid-row: 1/3;
        }
        &:nth-child(4){
          grid-column: 1/3;
        }
      }
      &:hover {
        filter: drop-shadow(0px 4px 30px rgba(114, 94, 137, 0.8));
      }
    }
    img {
      object-fit: contain;
      width: 100%;
      height: 100%;
    }
    h3 {
      font-weight: 700;
      font-size: 22px;
      line-height: 1.3;
      text-transform: uppercase;
      color: #FFFFFF;
      position: absolute;
      top: 40px;
      left: 50%;
      transform: translateX(-50%);
      text-align: center;
      width: 100%;
      @media(min-width:992px){
        font-size: 32px;
        line-height: 44px;
      }
    }
  }
}
</style>