<template>
  <section class="copyrights">
    <div class="container">
      <svg class="copyrights-logo" width="206" height="30" viewBox="0 0 206 30" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><rect width="206" height="30" fill="url(#pattern0)"/><defs><pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1"><use xlink:href="#image0_151_64" transform="translate(0 -0.00316092) scale(0.00172414 0.0118391)"/></pattern><image id="image0_151_64" width="580" height="85" xlink:href="data:image/png;base64,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"/></defs></svg>
      <p> © Copyright <span id="year"></span> Cyber Link</p>
    </div>
  </section>
</template>
<script>
  export default{
    methods: {
      currentDate() {
        const date = new Date(),
              currentDate = date.getFullYear();
        document.getElementById('year').innerHTML = currentDate;
      }
    },
    mounted() {
      this.currentDate()
    }
  }
</script>
<style lang="scss" scoped>
.copyrights {
  padding: 35px 0;
  background: #2A0E49;
  .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  p {
    font-weight: 400;
    font-size: 13px;
    line-height: 25px;
    color: #FFFFFF;
    @media(min-width:768px){
      font-size: 18px;
    }
  }
  &-logo {
    width: 150px;
    @media(min-width:768px){
      width: 206px;
    }
  }
}
</style>