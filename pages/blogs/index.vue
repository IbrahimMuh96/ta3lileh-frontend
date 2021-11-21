<template>
  <div id="index">
    <Navbar> </Navbar>
    <section class="blog-container">
      <div class="blogs-card">
        <div class="card" v-for="n in 4">
          <img src="../../assets/img/west-blog.jpg" alt="" />
          <div class="svg">
            <img src="../../assets/img/blog-card.svg" alt="" />
            <p class="text">
              what are you looking for what are you what are you looking for
              what are you what are you looking for what are you
            </p>
          </div>
        </div>
      </div>
      <div class="right-index">
        <div class="card mb-12">
          <div class="head">
            <h1>KEY WORDS</h1>
            <span class="bar bar-tags"></span>
          </div>
          <div class="tags">
            <a href="" class="tag">party</a>
            <a href="" class="tag">TICKET</a>
            <a href="" class="tag"> Adventure</a>
          </div>
        </div>

        <div class="card">
          <div class="head">
            <h1>RECENT POST</h1>
            <span class="bar"></span>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  layout: 'home',
}
</script>

<style lang="scss" scoped>
.blog-container {
  @apply justify-between mx-auto mt-11 flex flex-col;
  @media only screen and (min-width: 1111px) {
    @apply flex-row;
  }
  @media only screen and (min-width: 498px) {
    padding-left: 2.5rem;
    padding-right: 2.5rem;
  }

  max-width: 1818px;
}

.blogs-card{
  @apply grid grid-cols-3 gap-8 mr-8;
    .card{
      @apply max-w-full relative;
      border-radius: 15px;
      width: 30rem;
      img{
        border-radius: 15px;
      }
      .svg{
        position: relative;
margin-top: -10rem !important;
z-index: 2;
.text{
  position: absolute;
z-index: 3;
top: 7rem !important;
padding: 19px;
width: 19.5rem !important;
}
      }
    }
  }
 

.right-index {
  @apply flex flex-col relative;
   
  .bar {
    @apply bg-white block mt-2 w-1/2;
    height: 2px;
  }
  .card {
    @apply text-white px-7 py-6 max-w-full;
    width: 100% !important;
    @media only screen and (min-width: 1111px) {
      width: 368.91px !important;
    }
    border-radius: 9.41px;
    background: rgba(36, 36, 36, 0.9);
    .head {
      @apply relative mb-10;
      h1 {
        @apply tracking-widest text-xl;
      }
      .bar-tags {
        width: 33% !important;
      }
      .float-svg {
        @apply absolute;
        top: -6px;
        left: 72px;
      }
    }
    .recent-post {
      @apply flex items-center mb-10;
      img {
        @apply mr-3;
        width: 115px;
        height: 115px;
        border-radius: 10px;
      }
      .bar {
        margin-top: 12px !important;
        margin-bottom: 12px !important;
        width: 100% !important;
      }
      .date {
        @apply text-sm;
      }
    }
    .tags {
      @apply grid grid-cols-2 gap-7;
      .tag {
        @apply flex items-center justify-center text-white px-6 py-2 inline-flex;
        border-radius: 9.82px;
        background: linear-gradient(to right, #faab20 0%, #de158c 100%);
      }
    }
    
  }
}
</style>