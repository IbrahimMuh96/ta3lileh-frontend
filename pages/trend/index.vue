<template>
  <div id="index">
    <section class="home-page">
      <Navbar />
    </section>
    <section class="trend-landing section-container">
      <div class="left-section">
        <h1 class="title">TREND</h1>
        <p class="name">NAME</p>
        <p class="text">DFGHVBJKJHVBB FDFGHVBJKJHVBB FDFGHVBJKJHVBB</p>
        <div>
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
        <div class="arrows">
          <p>
            <span><i class="fas fa-chevron-right"></i></span>
            <span><i class="fas fa-chevron-right"></i></span>
            <span><i class="fas fa-chevron-right"></i></span>
          </p>
        </div>
        <span class="bar"></span>
      </div>

      <div class="right-section">
        <img src="../../assets/img/trend.jpg" alt="" />
      </div>
    </section>
    <section class="filters">
      <div class="float-img">
        <img src="../../assets/img/filter-float.svg" alt="" />
      </div>
      <div class="filter-container">
        <div class="input">
          <div>
            <span class="icon"><i class="fas fa-map-marker-alt"></i></span>
            <span class="label">Location</span>
          </div>
          <select name="" id="">
            <option value="">Amman</option>
          </select>
          <span class="arrow"><i class="fas fa-sort-down"></i></span>
        </div>
        <div class="input">
          <div>
            <span class="icon"><i class="fal fa-bullseye-arrow"></i></span>
            <span class="label">Category</span>
          </div>
          <select name="" id="">
            <option value="">Art</option>
          </select>
          <span class="arrow"><i class="fas fa-sort-down"></i></span>
        </div>
        <div class="input">
          <div>
            <span class="icon"><i class="fal fa-calendar-alt"></i></span>
            <span class="label">Date from</span>
          </div>
          <input type="date" />
          <span class="arrow"><i class="fas fa-sort-down"></i></span>
        </div>
        <div class="input">
          <div>
            <span class="icon"><i class="fal fa-calendar-alt"></i></span>
            <span class="label">Date to</span>
          </div>
          <input type="date" />
          <span class="arrow"><i class="fas fa-sort-down"></i></span>
        </div>
      </div>
      <div class="sort-container">
        <div class="input">
          <div>
            <span class="icon"><i class="fal fa-money-check-alt"></i></span>
            <span class="label">Price</span>
          </div>
        <div class="flex items-center">
          <span>Less</span>
            <label class="switch">
            <input type="checkbox" checked />
            <span class="slider round"></span>
          </label>
          <span>High</span>
        </div>
        </div>
        <div class="input">
          <div>
            <span class="icon"><i class="fas fa-star"></i></span>
            <span class="label">Rate</span>
          </div>
        <div class="flex items-center">
          <span>Less</span>
            <label class="switch">
            <input type="checkbox" checked />
            <span class="slider round"></span>
          </label>
          <span>High</span>
        </div>
        </div>
      </div>
    </section>
    <section class="section-container flex flex-col items-center">
      <div class="related-cards">
        <div class="card">
          <div class="summer-card">
            <img src="../../assets/img/summer.png" alt="" />
            <p class="name-container">Name of creator</p>
          </div>
          <div class="w-full px-4 py-2">
            <div class="card-head">
              <div class="stars">
                <span><i class="fal fa-star"></i></span>
                <span><i class="fal fa-star"></i></span>
                <span><i class="fal fa-star"></i></span>
                <span><i class="fal fa-star"></i></span>
                <span><i class="fal fa-star"></i></span>
              </div>
              <div>
                <img src="../../assets/img/related.svg" alt="" />
              </div>
            </div>
            <h1>NAME OF EVENT</h1>
            <p class="text">DFGHVBJKJHVBBFNcMNB</p>
            <div class="card-items">
              <p>
                <span><i class="fal fa-map-marker-smile"></i></span>
                <span>Location</span>
              </p>
              <p>
                <img src="../../assets/img/card-arrow.svg" alt="" />
              </p>
            </div>
            <div>
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
                <span class="bar"></span>
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="pagination">
        <a class="pag-btn">
          <span><i class="fal fa-arrow-left"></i></span>
          <span>BACK</span>
        </a>

        <a class="pag-btn">
          <span><i class="fal fa-arrow-right"></i></span>
          <span>NEXT</span>
        </a>
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
  .section-container {
    max-width: 1866px !important;
  }
  .trend-landing {
    @apply flex justify-between mb-20 text-white;

    .left-section {
      @apply mr-12;
      .title {
        font-family: 'LuckiestGuy';
        @apply mb-8;
        font-size: 6rem;
      }
      .name {
        font-family: 'LuckiestGuy';
        @apply mb-4 ml-6;
        font-size: 3rem;
      }
      .text {
        @apply ml-6 mb-8;
      }
      .arrows {
        @apply flex justify-end mb-8;
        font-size: 26px;
        background: -webkit-linear-gradient(#faab20 0%, #de158c 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }
      .detail {
        @apply flex items-center font-light mb-6 ml-6;
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
        .text {
          @apply mb-4;
          font-size: 14px;
        }
        .data-time {
          @apply text-white flex items-center justify-center;
          padding: 2px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
          .data-container {
            @apply px-2 text-white;
            width: 66px;
            background: rgba(36, 36, 36, 1);
            border-radius: 15px;
          }
        }
      }
      .bar {
        height: 3px;
        width: 100%;
        @apply flex ml-2;
        background: linear-gradient(to right, #faab20 0%, #de158c 100%);
      }
    }
    .right-section {
      @apply w-full  aspect-w-16 aspect-h-6;
      max-width: 77rem;
      border-radius: 25px;
      img {
        @apply w-full bg-cover bg-center aspect-w-16 aspect-h-9 max-h-full;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2),
          0 6px 20px 0 rgba(0, 0, 0, 0.19);
        height: 585.75px;
        border-radius: 25px;
      }
    }
  }

  .filters {
    @apply flex justify-between mx-auto;
    max-width: 76rem;

     .filter-container {
      @apply p-6 grid grid-cols-2 gap-8 max-w-full;
      width: 800px;
      border-radius: 15px;
      background: rgba(206, 205, 205, 0.7);
      .input {
        @apply px-4 py-2 flex items-center justify-between relative;
        border-radius: 6px;
        background: rgba(206, 205, 205, 0.9);
        .label {
          @apply mr-4;
        }
        .icon {
          @apply mr-4;
        }

        input,
        select {
          @apply px-10 py-1 outline-none select-none;
          width: 203px;
          border-radius: 15px;
          background: linear-gradient(to right, #faab20 0%, #de158c 100%);
        }

        .arrow {
          @apply absolute text-white;
          right: 30px;
          top: 9px;
          font-size: 1rem;
        }
        .switch {
          @apply mx-4;
          position: relative;
          display: inline-block;
          width: 60px;
          height: 34px;
        }

        .switch input {
          opacity: 0;
          width: 0;
          height: 0;
        }

        .slider {
          position: absolute;
          cursor: pointer;
          top: 0;
          left: 0;
          right: 0;
          bottom: 0;
          background-color: #ccc;
          box-shadow: 0 0 1px #de158c;

          -webkit-transition: 0.4s;
          transition: 0.4s;
        }

        .slider:before {
          position: absolute;
          content: '';
          height: 26px;
          width: 26px;
          left: 4px;
          bottom: 4px;
          background-color: white;
          -webkit-transition: 0.4s;
          transition: 0.4s;
        }

        input:checked + .slider {
          background: linear-gradient(to right, #faab20 0%, #de158c 100%);
        }

        input:focus + .slider {
          box-shadow: 0 0 1px #de158c;
        }

        input:checked + .slider:before {
          -webkit-transform: translateX(26px);
          -ms-transform: translateX(26px);
          transform: translateX(26px);
        }

        /* Rounded sliders */
        .slider.round {
          border-radius: 34px;
        }

        .slider.round:before {
          border-radius: 50%;
        }
      }
    }
    .float-img{
      @apply absolute;
      top: 37rem;
      left: 7rem;
    }
    .sort-container {
      @apply p-6 grid grid-cols-1 gap-8;
      border-radius: 15px;
      background: rgba(206, 205, 205, 0.7);
      .input {
        @apply px-4 py-2 flex items-center justify-between relative;
        border-radius: 6px;
        background: rgba(206, 205, 205, 0.9);
        .label {
          @apply mr-4;
        }
        .icon {
          @apply mr-4;
        }

        input,
        select {
          @apply px-10 py-1 outline-none select-none;
          width: 203px;
          border-radius: 15px;
          background: linear-gradient(to right, #faab20 0%, #de158c 100%);
        }

        .arrow {
          @apply absolute text-white;
          right: 30px;
          top: 9px;
          font-size: 1rem;
        }
        .switch {
          @apply mx-4;
          position: relative;
          display: inline-block;
          width: 60px;
          height: 34px;
        }

        .switch input {
          opacity: 0;
          width: 0;
          height: 0;
        }

        .slider {
          position: absolute;
          cursor: pointer;
          top: 0;
          left: 0;
          right: 0;
          bottom: 0;
          background-color: #ccc;
          box-shadow: 0 0 1px #de158c;

          -webkit-transition: 0.4s;
          transition: 0.4s;
        }

        .slider:before {
          position: absolute;
          content: '';
          height: 26px;
          width: 26px;
          left: 4px;
          bottom: 4px;
          background-color: white;
          -webkit-transition: 0.4s;
          transition: 0.4s;
        }

        input:checked + .slider {
          background: linear-gradient(to right, #faab20 0%, #de158c 100%);
        }

        input:focus + .slider {
          box-shadow: 0 0 1px #de158c;
        }

        input:checked + .slider:before {
          -webkit-transform: translateX(26px);
          -ms-transform: translateX(26px);
          transform: translateX(26px);
        }

        /* Rounded sliders */
        .slider.round {
          border-radius: 34px;
        }

        .slider.round:before {
          border-radius: 50%;
        }
      }
    }
  }
  .related-cards {
    .card {
      @apply flex flex-col items-center text-white;

      .card-head {
        @apply flex items-center justify-between w-full mb-2;
      }

      .card-items {
        @apply flex items-center justify-between mb-4;
      }
      border-radius: 15px;
      background: rgba(36, 36, 36, 1);
      h1 {
        @apply text-2xl mb-2;
      }
      .text {
        @apply mb-4;
        font-size: 14px;
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
        .bar {
          height: 1px;
          width: 100%;
          @apply flex ml-2;
          background: linear-gradient(to right, #faab20 0%, #de158c 100%);
        }
        .data {
          @apply text-white px-4 flex items-center justify-center;
          padding-top: 1px;
          padding-bottom: 1px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
        }
        .text {
          @apply mb-4;
          font-size: 14px;
        }
        .data-time {
          @apply text-white flex items-center justify-center;
          padding: 2px;
          border-radius: 15px;
          background: linear-gradient(#faab20 0%, #de158c 100%);
          .data-container {
            @apply px-2 text-white;
            width: 66px;
            background: rgba(36, 36, 36, 1);
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
        @apply relative text-white;

        .name-container {
          @apply px-3 py-0.5 absolute;
          bottom: 0;
          right: 0;

          border-radius: 15px 0px 15px 0px;

          background: black;
        }
        .price {
          border-radius: 5px;
          @apply flex bg-white  px-2 py-1;
        }
      }
    }
  }

  .pagination {
    @apply flex  items-center justify-center mt-8 mb-8;

    .pag-btn {
      @apply mx-4 flex flex-col items-center justify-center text-white cursor-pointer;

      span:nth-child(1) {
        @apply flex items-center justify-center text-white text-2xl rounded-full;
        width: 44.42px;
        height: 41.72px;
        background: linear-gradient(#faab20 0%, #de158c 100%);
      }
      span:nth-child(2) {
        @apply mt-1;
      }
    }
  }
}
</style>