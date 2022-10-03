<template>
  <section class="contact">
    <div class="container">
      <h2>связаться с нами</h2>
      <div class="contact-wrap">
        <div class="contact-info">оставьте заявку и наш специалист перезвонит Вам в течение 5 мин <br><br> <span>пн-пт 10:00 - 19:00</span> <br> <span>сб-вс 11:00 - 18:00</span></div>
        <form class="contact-form" @submit="submitForm">
          <div class="contact-form-field">
            <input type="text" placeholder="Ваше имя*" v-model="name" required>
            <input type="tel" placeholder="Ваш телефон*" v-model="phone" required>
          </div>
          <input type="email" placeholder="Электронная почта" v-model="email" required>
          <button
            type="submit"
            :disabled="this.name === null || this.email === null || this.phone === null "
          >
            отправить
          </button>
        </form>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      name: null,
      email: null,
      phone: null,
    }
  },
  methods: {
    submitForm(e) {
      e.preventDefault()
      console.log('submit');
    }
  }
}

</script>
<style lang="scss">
.contact {
  padding: 60px 0;
  background: #3C1D58;
  h2 {
    font-weight: 700;
    font-size: 22px;
    line-height: 1.3px;
    text-transform: uppercase;
    color: #FFFFFF;
    margin-bottom: 20px;
    @media(min-width:992px){
      font-size: 32px;
      line-height: 44px;
    }
  }
  &-wrap {
    @media(min-width:992px){
      display: flex;
    }
  }
  &-info {
    font-weight: 400;
    font-size: 18px;
    line-height: 25px;
    color: #FFFFFF;
    margin-bottom: 50px;
    @media(min-width:992px){
      margin-bottom: 0;
      max-width: 392px;
      margin-right: 123px;
    }
    span {
      color: #BEA8D7;
    }
  }
  &-form {
    width: 100%;
    &-field {
      @media(min-width:768px){
        display: flex;
        justify-content: space-between;
        &>input {
          &:first-child {
            max-width: 41.22%;
            flex-basis: 41.22%;
          }
          &:last-child {
            max-width: 55.92%;
            flex-basis: 55.92%;
          }
        }
      }
    }
    input {
      width: 100%;
      height: 54px;
      background: rgba(114, 94, 137, 0.5);
      border: none;
      outline: none;
      margin-bottom: 20px;
      padding: 15px 30px;
      font-weight: 400;
      font-size: 16px;
      line-height: 25px;
      color: #fff;
      @media(min-width:768px){
        font-size: 18px;
      }
      &::placeholder {
        color: #BEA8D7;
      }
      &.error {
        border: 1px solid #FF002E;
      }
    }
    button {
      width: 100%;
      border: 1px solid #DBB3FE;
      background: none;
      height: 54px;
      font-weight: 700;
      font-size: 20px;
      line-height: 27px;
      display: flex;
      align-items: center;
      justify-content: center;
      text-transform: uppercase;
      color: #FFFFFF;
      transition: 0.5s ease;
      padding: 0;
      @media(min-width:768px){
        max-width:289px;
        margin-left: auto;
      }
      &:hover {
        background: #DBB3FE;
        box-shadow: 0px 9px 30px rgba(220, 199, 255, 0.3);
      }
      &:active {
        background: #BEA8D7;
        box-shadow: 0px 4px 30px rgba(220, 199, 255, 0.3);
        border: 1px solid #BEA8D7;
      }
      &:disabled {
        background: #A9A9A9;
        border: 1px solid #A9A9A9;
        &:hover{
          box-shadow: none;
        }
      }
    }
  }
}
</style>