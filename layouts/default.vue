<template>
  <main>
    <Nuxt />
  </main>
</template>

<style lang="scss">
* {
  font-family: 'Open Sans', sans-serif;
}

.container {
  width: 100%;
  padding-left: 15px;
  padding-right: 15px;
  margin-left: auto;
  margin-right: auto;
  position: relative;
  @media (min-width: 768px) {
    max-width: 768px;
    padding-left: 30px;
    padding-right: 30px;
  }
  @media (min-width: 992px) {
    max-width: 992px;
  }
  @media (min-width: 1200px) {
    max-width: 1200px;
  }
  @media (min-width: 1400px) {
    max-width: 1276px;
  }
}
</style>