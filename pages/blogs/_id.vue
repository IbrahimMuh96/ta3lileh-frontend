<template>
  <div id="index">
    <Navbar> </Navbar>
    <section class="blog-container">
      <div class="blog-body">
        <img src="../../assets/img/west.jpg" alt="" />
        <div class="body">
          <div class="details">
            <p class="title">
              <span>The best activities to do in spring</span>
              <span class="bar"></span>
            </p>
            <p class="date">
              <span><i class="fal fa-calendar-alt"></i></span>
              <span>11 JUN 2021</span>
            </p>
          </div>
          <p class="blog-text">
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam
            nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat
            volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation
            ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo
            consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate
            velit esse molestie consequat, vel illum dolore eu feugiat nulla
            facilisis at vero eros et accumsan et iusto odio dignissim qui
            blandit praesent luptatum zzril delenit augue duis dolore te feugait
            nulla facilisi. Lorem ipsum dolor sit amet, cons ectetuer adipiscing
            elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore
            magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis
            nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip
            ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetuer
            adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet
            dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam,
            quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut
            aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in
            hendrerit in vulputate velit esse molestie consequat, vel illum
            dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto
            odio dignissim qui blandit praesent luptatum zzril delenit augue
            duis dolore te feugait nulla facilisi. Lorem ipsum dolor sit amet,
            cons ectetuer adipiscing elit, sed diam nonummy nibh euismod
            tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi
            enim ad minim veniam, quis nostrud exerci tation ullamcorper
            suscipit lobortis nisl ut aliquip ex ea commodo consequat. Lorem
            ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy
            nibh euismod tincidunt ut laoreet dolore magna aliquam erat
            volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation
            ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo
            consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate
            velit esse molestie consequat, vel illum dolore eu feugiat nulla
            facilisis at vero eros et accumsan et iusto odio dignissim qui
            blandit praesent luptatum zzril delenit augue duis dolore te feugait
            nulla facilisi. Lorem ipsum dolor sit amet, cons ectetuer adipiscing
            elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore
            magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis
            nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip
            ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetuer
            adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet
            dolore
          </p>
        </div>
      </div>
      <div class="right-index">
        <div class="card mb-12">
          <div class="head">
            <h1>tags</h1>
            <span class="bar bar-tags"></span>
            <span class="float-svg"
              ><img src="../../assets/img/tags.svg" alt=""
            /></span>
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

          <nuxt-link to="/" class="recent-post" v-for="n in 4" :key="n.id">
            <img src="../../assets/img/westlife.png" alt="" />
            <div>
              <p class="title">The best activities to do in spring</p>
              <span class="bar"></span>
              <p class="date">
                <span><i class="fal fa-calendar-alt"></i></span>
                <span>11 JUN 2021</span>
              </p>
            </div>
          </nuxt-link>

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
.blog-container{
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
.blog-body {
  @apply w-full mr-6 text-white mb-12;
  background: rgba(36, 36, 36, 0.9);
  max-width: 100%;

  border-radius: 20px;

  img {
    @apply bg-cover w-full shadow;
    max-height: 639px;
    width: 100%;
    border-radius: 20px;
  }
  .body {
    @apply p-6;
    .details {
      @apply flex justify-between items-center mb-6;
       @media only screen and (max-width: 637px) {
       @apply flex-col;
      }
      .title {
        @apply flex flex-col;
        span:nth-child(1) {
          @apply ml-7;
        }
        .bar {
          @apply max-w-full bg-white mt-3 mb-3;
          height: 1px;
          width: 19rem;
        }
      }
      .date {
        @apply text-sm;
      }
    }
    .blog-text{
      line-height: 2rem;
    }
  }
}

.right-index {
  @apply flex flex-col relative;
  .steps {
    @apply relative flex-col flex items-center mb-9;
    span {
      @apply absolute text-white text-xl;
    }

    .first_step {
      top: 32px;
      left: 52px;
    }
    .second_step {
      top: 32px;
    }
    .third_step {
      top: 32px;
      right: 52px;
    }
  }
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
    .pay {
      @apply mt-5;
      margin-left: 48px;
    }
    .confirm-btn {
      @apply w-full;
      a {
        @apply rounded-full w-full flex items-center justify-center py-1 mt-10;
        background: linear-gradient(to right, #f9aa20 0%, #dd158b 100%);
      }
    }
  }
}
</style>