<template>
  <section class="banner">
    <div class="container">
      <h1>Комплексные поставки IT-оборудования напрямую от производителя</h1>
      <form>
        <svg width="28" height="28" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M22.9339 23.4187L15.7922 16.2769C16.9004 14.8442 17.4999 13.0925 17.4999 11.25C17.4999 9.04447 16.6392 6.97648 15.0827 5.41724C13.5262 3.858 11.4527 3 9.24996 3C7.04722 3 4.97373 3.86075 3.41724 5.41724C1.858 6.97373 1 9.04447 1 11.25C1 13.4527 1.86075 15.5262 3.41724 17.0827C4.97373 18.6419 7.04447 19.4999 9.24996 19.4999C11.0925 19.4999 12.8414 18.9004 14.2742 17.7949L21.4159 24.9339C21.4369 24.9549 21.4617 24.9715 21.4891 24.9828C21.5165 24.9942 21.5458 25 21.5754 25C21.605 25 21.6344 24.9942 21.6617 24.9828C21.6891 24.9715 21.714 24.9549 21.7349 24.9339L22.9339 23.7377C22.9549 23.7167 22.9715 23.6919 22.9828 23.6645C22.9942 23.6371 23 23.6078 23 23.5782C23 23.5485 22.9942 23.5192 22.9828 23.4918C22.9715 23.4645 22.9549 23.4396 22.9339 23.4187ZM13.6059 15.6059C12.44 16.7692 10.8945 17.4099 9.24996 17.4099C7.60547 17.4099 6.05998 16.7692 4.89398 15.6059C3.73074 14.44 3.08999 12.8945 3.08999 11.25C3.08999 9.60547 3.73074 8.05723 4.89398 6.89398C6.05998 5.73074 7.60547 5.08999 9.24996 5.08999C10.8945 5.08999 12.4427 5.72799 13.6059 6.89398C14.7692 8.05998 15.4099 9.60547 15.4099 11.25C15.4099 12.8945 14.7692 14.4427 13.6059 15.6059Z" fill="white"/></svg>
        <input type="text" placeholder="Сервер для решения...">
        <button type="submit">Найти</button>
      </form>
    </div>
  </section>
</template>
<style lang="scss" scoped>
.banner {
  background-image: url('@/assets/img/bg.png');
  background-color: #2A0E49;
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 100vh;
  position: relative;
  @media(min-width:1200px){
    background-size: contain;
  }
  .container {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
     align-items: center;
  }
  &:before{
    content: "";
    width: 100%;
    height: 100%;
    background: rgba(114, 94, 137, 0.05);
    backdrop-filter: blur(10px);
    position: absolute;
    top: 0;
    left: 0;
    z-index: 0;
  }
  h1 {
    font-weight: 700;
    font-size: 30px;
    line-height: 1.3;
    text-align: center;
    color: #FFFFFF;
    margin-bottom: 30px;
    @media(min-width:768px){
      font-size: 48px;
      line-height: 65px;
    }

  }
  form {
    display: flex;
    max-width: 804px;
    margin: 0 auto;
    position: relative;
    input {
      display: block;
      width:100%;
      height: 54px;
      background: rgba(114, 94, 137, 0.5);
      backdrop-filter: blur(20px);
      border: none;
      outline: none;
      font-size: 16px;
      line-height: 25px;
      color: #fff;
      padding-left: 58px;
      @media(min-width:768px){
        font-size: 18px;
        padding-left: 78px;
      }
      &::placeholder {
        color: #BEA8D7;
      }
    }
    svg {
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      left: 10px;
      z-index: 2;
      @media(min-width:768px){
        left: 30px;
      }
    }
    button {
      padding: 0;
      display: block;
      border: none;
      font-weight: 700;
      font-size: 16px;
      line-height: 27px;
      display: flex;
      align-items: center;
      text-align: center;
      text-transform: uppercase;
      justify-content: center;
      color: #FFFFFF;
      width: 100px;
      height: 54px;
      background: #725E89;
      transition: 0.5s ease;
      @media(min-width:768px){
        width: 140px;
        font-size: 20px;
      }
      &:hover,
      &:active {
        filter: drop-shadow(0px 9px 30px rgba(220, 199, 255, 0.3));
        background: #DBB3FE;
      }
    }
  }
}
</style>