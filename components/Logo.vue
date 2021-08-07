<template>
  <div class="logo">
    <img src="../assets/img/logo.svg" alt="" />
    <img src="../assets/img/subLogo.svg" alt="" />
  </div>
</template>

<style lang="scss" scoped>
.logo {
  img:nth-child(1) {
    @apply hidden;
    @media only screen and (min-width: 380px) {
      @apply flex;
    }
  }
  img:nth-child(2) {
    @apply flex;
    @media only screen and (min-width: 380px) {
      @apply hidden;
    }
  }
}
</style>