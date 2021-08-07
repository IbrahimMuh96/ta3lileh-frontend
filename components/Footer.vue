<template>
  <div id="footer">
    <div class="container">
      <div class="col">
         <div class="head">
          <div class="item">
            ABOUT
            <span class="bar"></span>
          </div>
        </div>
        <div class="item">
          <nuxt-link to="/about-us"> - About us </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/policy"> - Privacy policy </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/Term"> - Term & Conditions </nuxt-link>
        </div>
      </div>

      <div class="col">
        <div class="head">
          <div class="item">
            support
            <span class="bar"></span>
          </div>
        </div>
        <div class="item">
          <nuxt-link to="/account"> - My account </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/contact"> - Contact us </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/write"> - Write for us </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/ "> - How it work </nuxt-link>
        </div>
      </div>
      <div class="col">
         <div class="head">
          <div class="item">
            Features
            <span class="bar"></span>
          </div>
        </div>
        <div class="item">
          <nuxt-link to="/features"> - Features </nuxt-link>
        </div>
      </div>
      <div class="social-col">
        <img src="../assets/img/footer-logo.png" alt="" />
        <div class="icons">
            <a href="" target="_blank"><i class="fab fa-instagram"></i></a>
            <a href="" target="_blank" ><i class="fab fa-facebook-f"></i></a>
            <a href="" target="_blank"><i class="fab fa-tiktok"></i></a>
        </div>
        <p>OUR SOCIAL MEDIA ACCONTS</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#footer {
    @apply py-8;
  background: rgba(36, 36, 36, 0.5);
  .container {
    @apply text-white grid grid-cols-1 px-6 justify-items-center place-content-center gap-y-10;
    @media only screen and (min-width: 437px) {
            @apply grid-cols-2 ;
       }
    @media only screen and (min-width: 1076px) {
            @apply grid-cols-4 ;
       }
    .col {
      @apply flex flex-col;
      .head {
        @apply flex justify-start;

        .item {
          @apply text-xl font-semibold mb-5 flex-col flex items-center justify-center relative text-center;
          .bar {
            @apply absolute;
            bottom: -4px;
            width: 5rem;
            height: 1px;
            background: linear-gradient(#faab20 0%, #de158c 100%);
          }
        }
      }
      .item {
        @apply mb-2;
      }
      @media only screen and (max-width: 437px) {
             width: 146px;
       }
      &:nth-child(3){
          width: 145px;
          @media only screen and (min-width: 1076px) {
             width: 176px;
       } 
      }
    }
    .social-col{
        @apply flex flex-col justify-center;
          @media only screen and (min-width: 1076px) {
            @apply items-center;
       }
        img{
            @apply mb-2;
        width: 64.87px;
         }
         .icons{
             @apply flex items-center mb-2;
             a{
                 @apply mx-2;
             }
         }
         p{
             @apply hidden;
              @media only screen and (min-width: 1076px) {
            @apply flex;
       }
         }
         @media only screen and (max-width: 437px) {
             width: 146px;
       }
    }
  }
}
</style>