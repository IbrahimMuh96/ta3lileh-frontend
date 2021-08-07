<template>
  <div id="index">
    <Navbar> </Navbar>
     <section class="section-container">
    <div class="page-form">
      <div class="title">
        <img src="../../assets/img/personal-info.svg" alt="" />
      </div>
        <div class="index-form">
        <div class="notAuth">
          <div class="head">
            <p>Log In To View Your Account</p>
            <span class="bar" style="height:3px"></span>
          </div>
          
          <div class="message">
              <h1>You Dont Have Account</h1>
              <a >Log in</a>
          </div>
        </div>


        <div class="float-img">
          <img src="../../assets/img/personal-float.svg" alt="" />
        </div>
      </div>
     </div>
     </section>
  </div>
</template>

<style lang="scss" scoped>
.index-form{

}
</style>
<script>
export default {
  layout: 'home',
}
</script>