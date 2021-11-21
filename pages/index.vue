<template>
  <div id="index">
    <section class="home-page">
      <Navbar />
    </section>
    
    <section class="section-container flex flex-col items-center">
      <h1>what are you looking for ?</h1>

      <div class="comming-cards">
        <div class="card">
          <div class="summer-card">
            <img src="../assets/img/summer.png" alt="" />
            <div class="price-container">
              <p class="price">
                <span>30</span>
                <sub class="ml-1">jd</sub>
              </p>
            </div>
          </div>
          <div class="event-detail">
            <h1>EVENTS NAME</h1>
            <div>
              <p class="detail">
                <span class="icon"
                  ><i class="fal fa-map-marker-smile"></i
                ></span>
                <span>Amaan- Jordan</span>
              </p>
              <p class="detail">
                <span class="icon"><i class="fal fa-user"></i></span>
                <span>Name of creator</span>
              </p>
              <p class="detail">
                <span class="icon"><i class="fal fa-calendar-alt"></i></span>
                <span class="data">
                  25
                  <sub class="ml-1">jan</sub>
                </span>
                <span class="data-time ml-2">
                  <span class="data-container">
                    6:00
                    <sub class="">pm</sub>
                  </span>
                </span>
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="available-cards">
        <div class="available-card">
          <div class="summer-card">
            <img src="../assets/img/summer.png" alt="" />
            <div class="price-container">
              <p class="price">
                <span>30</span>
                <sub class="ml-1">jd</sub>
              </p>
            </div>
          </div>
          <div class="card">
            <div class="event-detail">
              <h1>EVENTS NAME</h1>

              <div>
                <p class="detail">
                  <span class="icon"
                    ><i class="fal fa-map-marker-smile"></i
                  ></span>
                  <span>Amaan- Jordan</span>
                </p>
                <p class="detail">
                  <span class="icon"><i class="fal fa-user"></i></span>
                  <span>Name of creator</span>
                </p>
                <p class="detail">
                  <span class="icon"><i class="fal fa-calendar-alt"></i></span>
                  <span class="data">
                    25
                    <sub class="ml-1">jan</sub>
                  </span>
                  <span class="data-time ml-2">
                    <span class="data-container">
                      6:00
                      <sub class="">pm</sub>
                    </span>
                  </span>
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="most-booked">
        <div class="card">
          <div class="summer-card">
            <img src="../assets/img/summer.png" alt="" />
          </div>
          <div class="event-detail">
            <h1>EVENTS NAME</h1>
            <div>
              <p class="about-title">
                <span>About</span>
                <span class="bar"></span>
              </p>
              <p class="detail">
                <span class="icon"
                  ><i class="fal fa-map-marker-smile"></i
                ></span>
                <span>Amaan- Jordan</span>
              </p>
              <p class="detail">
                <span class="icon"><i class="fal fa-user"></i></span>
                <span>Name of creator</span>
              </p>
              <p class="detail">
                <span class="icon"><i class="fal fa-calendar-alt"></i></span>
                <span class="data">
                  25
                  <sub class="ml-1">jan</sub>
                </span>
                <span class="data-time ml-2">
                  <span class="data-container">
                    6:00
                    <sub class="">pm</sub>
                  </span>
                </span>
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="loking-for">
          <div class="cards">
              <div class="card">
                <div></div>
                <div></div>
                <div class="number">
                  <span class="bar"></span>
                  <span>55</span>
                  <span class="bar"></span>
                </div>
              </div>
          </div>
      </div>
    </section>

    <section class="section-container clients">
        <div class="clients-container">
          <div>

          </div>
          <div class="our-clients">
               <img src="../assets/img/Roya.png" alt="" />
                <img src="../assets/img/Roya.png" alt="" />
                 <img src="../assets/img/Roya.png" alt="" />
                  <img src="../assets/img/Roya.png" alt="" />
          </div>

          <div class="blogs-card">
              <div class="card">
                <img src="../assets/img/west-blog.jpg" alt="" />
                <div class="svg">
                  <img src="../assets/img/blog-card.svg" alt="" />
                  <p class="text">what are you looking for what are you
                    what are you looking for what are you
                    what are you looking for what are you
                  </p>
                </div>
              </div>
          </div>
        </div>
    </section>
    <Footer />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
#index {
  .comming-cards {
    @apply mb-32;
    .card {
      @apply py-8 flex items-center;
      width: 27rem;
      border-radius: 15px;
      background: rgba(206, 205, 205, 0.7);
      h1 {
        @apply text-2xl mb-5;
      }
      .detail {
        @apply flex items-center font-light mb-3;
        i {
          @apply mr-3;
          font-size: 24px;
        }
        .icon {
          width: 2rem;
        }
        .data {
          @apply text-white px-4 flex items-center justify-center;
          padding-top: 1px;
          padding-bottom: 1px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
        }
        .data-time {
          @apply text-white flex items-center justify-center;
          padding: 2px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
          .data-container {
            @apply px-2 text-black;
            background: rgba(206, 205, 205, 0.8);
            border-radius: 15px;
          }
        }
      }

      .event-detail {
        @apply flex flex-col items-center;
      }

      .summer-card {
        @apply relative;
        margin-left: -10rem;
        margin-right: 4rem;
        .price-container {
          @apply p-0.5 absolute;
          top: 10px;
          left: 8px;
          border-radius: 5px;

          background: linear-gradient(#faab20 0%, #de158c 100%);
        }
        .price {
          border-radius: 5px;
          @apply flex bg-white  px-2 py-1;
        }
      }
    }
  }
  .most-booked {
    .card {
      @apply pb-8 flex flex-col items-center;

      border-radius: 15px;
      background: rgba(206, 205, 205, 0.7);
      h1 {
        @apply text-2xl mb-5;
      }
      .detail {
        @apply flex items-center font-light mb-3;
        i {
          @apply mr-3;
          font-size: 24px;
        }
        .icon {
          width: 2rem;
        }
        .data {
          @apply text-white px-4 flex items-center justify-center;
          padding-top: 1px;
          padding-bottom: 1px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
        }
        .data-time {
          @apply text-white flex items-center justify-center;
          padding: 2px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
          .data-container {
            @apply px-2 text-black;
            background: rgba(206, 205, 205, 0.8);
            border-radius: 15px;
          }
        }
      }

      .event-detail {
        @apply flex flex-col;
        .about-title {
          @apply mb-4;
          .bar {
            @apply block;
            height: 1px;
            width: 3.7rem;
            background: linear-gradient(to right, #faab20 0%, #de158c 100%);
          }
        }
      }

      .summer-card {
        @apply relative mb-4;

        .price-container {
          @apply p-0.5 absolute;
          top: 10px;
          left: 8px;
          border-radius: 5px;

          background: linear-gradient(#faab20 0%, #de158c 100%);
        }
        .price {
          border-radius: 5px;
          @apply flex bg-white  px-2 py-1;
        }
      }
    }
  }
  .available-cards {
    @apply mb-32;
    .available-card{
        @apply flex flex-col items-center;
    }
    .summer-card {
      @apply relative;
      img{
          width: 24rem;
          margin-bottom: -1rem;
      }

      .price-container {
        @apply p-0.5 absolute;
        top: 10px;
        left: 8px;
        border-radius: 5px;

        background: linear-gradient(#faab20 0%, #de158c 100%);
      }
      .price {
        border-radius: 5px;
        @apply flex bg-white  px-2 py-1;
      }
    }
    .card {
      @apply py-8 flex flex-col justify-center items-center;
      width: 16rem;
      height: 19rem;
      border-radius: 15px;
      background: rgba(206, 205, 205, 0.7);
      h1 {
        @apply text-2xl mb-5;
      }
      .detail {
        @apply flex items-center font-light mb-3;
        i {
          @apply mr-3;
          font-size: 24px;
        }
        .icon {
          width: 2rem;
        }
        .data {
          @apply text-white px-4 flex items-center justify-center;
          padding-top: 1px;
          padding-bottom: 1px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
        }
        .data-time {
          @apply text-white flex items-center justify-center;
          padding: 2px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
          .data-container {
            @apply px-2 text-black;
            background: rgba(206, 205, 205, 0.8);
            border-radius: 15px;
          }
        }
      }

      .event-detail {
        @apply flex flex-col items-center;
      }
    }
  }
  .loking-for{
    .cards{
      .card{
        @apply border border-white mt-12 flex flex-col items-center relative;
        width: 122.38px;
         height: 122.38px;
         border-radius: 5px;

        div:nth-child(1){
          background: rgba(36, 36, 36, 0.7);
          height: 50%;
          width: 100%;
        }
        div:nth-child(2){
          background: rgba(190, 190, 190, 0.5);
           height: 50%;
          width: 100%;
        }
        .number{
          @apply flex items-center justify-between text-white text-6xl absolute w-full;
          top: 29px;
        }
        .bar{
         height: 21px;
          width: 6px;
          background: linear-gradient(#faab20 0%, #de158c 100%);

        }
      }
    }
  }
  .clients{
    .clients-container{
      @apply py-5 px-3 w-full;
    background: rgba(36, 36, 36, 0.9);
    .our-clients{
      @apply py-5 px-7 flex justify-between;
      background: #d2d2d2;
      border-radius: 15px;

      img{
       width: 9rem;
       height: 9rem;
      }

    }
  }
  }
}
</style>