<template>
  <div>
    <nav id="nav">
      <div>
        <nuxt-link to="/">
          <Logo />
        </nuxt-link>
      </div>
      <div class="nav-items links">
        <div class="item">
          <nuxt-link class="active-item" to="/">
            homepage
            <span class="active"></span>
          </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/blogs">
            blogs
            <span class="active"></span>
          </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/events">
            events
            <span class="active"></span>
          </nuxt-link>
        </div>
        <div class="item">
          <nuxt-link to="/contact">
            contact us
            <span class="active"></span>
          </nuxt-link>
        </div>
      </div>
      <div class="nav-items">
        <div class="input-append">
          <form action="">
            <input type="text" placeholder="search..." />
            <div class="btn-search">
              <button type="submit">
                <img src="../assets/img/search.png" alt="" />
              </button>
              <span class="bar"></span>
            </div>
          </form>
        </div>
        <div class="shop">
          <nuxt-link to="">
            <img src="../assets/img/shop.png" alt="" />
          </nuxt-link>
        </div>
        <div class="join-us">
          <a  @click="selectAuth('SIGN UP')">join us</a>
        </div>
        <div >
          <a class="btn" @click="selectAuth('LOG IN')">log in</a>
        </div>
          <div class="side-btn">
              <a @click="displaySideNav=!displaySideNav" class="cursor-pointer">
                <i class="fas fa-bars"></i>
              </a>
            </div>
      </div>
    </nav>
    <div id="auth" v-if="displayAuth">
      <div class="backdrop" @click="displayAuth=''"></div>
      <div class="auth-form h-full" :class="{'login-form':displayAuth=='LOG IN','sign-form':displayAuth=='SIGN UP'}">
          <div class="auth-btns">
            <a  :class="{'active':displayAuth=='SIGN UP','btn':displayAuth!='SIGN UP'}" @click="selectAuth('SIGN UP')">SIGN UP</a>
            <a   :class="{'active':displayAuth=='LOG IN','btn':displayAuth!='LOG IN'}" @click="selectAuth('LOG IN')">LOG IN</a>
          </div>
        <form action="" v-if="displayAuth==='LOG IN'">
          <div class="auth-input">
            <input type="email" placeholder="E-MAIL ADDRESS" />
            <span>
                <svg xmlns="http://www.w3.org/2000/svg" width="19.826" height="14.317" viewBox="0 0 14.826 9.317">
                    <g id="Group_27816" data-name="Group 27816" transform="translate(-785.538 -378.579)">
                        <path id="Path_202457" data-name="Path 202457" d="M792.938,383.516l-6.4-4.937h12.831Z" fill="#545454"/>
                        <path id="Path_202458" data-name="Path 202458" d="M790.717,383.1l-5.179,4.224V379.11Z" fill="#545454"/>
                        <path id="Path_202459" data-name="Path 202459" d="M791.554,383.748l1.382,1.065,1.457-1.12,5.06,4.2H786.468Z" fill="#545454"/>
                        <path id="Path_202460" data-name="Path 202460" d="M795.23,383.051l5.134-3.944v8.206Z" fill="#545454"/>
                    </g>
                    </svg>
            </span>
           </div>
          <div class="auth-input">
            <input type="password" placeholder="PASSWORD" />
            <span>
                <svg xmlns="http://www.w3.org/2000/svg" width="15.685" height="18.27" viewBox="0 0 10.685 13.27">
                    <g id="Group_27805" data-name="Group 27805" transform="translate(-787.115 -434.484)">
                        <path id="Path_202455" data-name="Path 202455" d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z" fill="#545454"/>
                    </g>
                </svg>
            </span>
          </div>
          <div class="auth-submit">
            <button type="submit">LOG IN</button>

               <div class="mt-4">
                  <span>
                    <div class="checkbox">
                        <input id="check1" type="checkbox" name="check" value="check1">
                        <label for="check1">Remember me</label>
                    </div>                        
                  </span>

                  <nuxt-link to="">Forget Password?</nuxt-link>
              </div>
          </div>
        </form>
        <form action="" v-if="displayAuth==='SIGN UP'">
          <div class="auth-input">
            <input type="text" placeholder="USER NAME" />
            <span>
                <svg xmlns="http://www.w3.org/2000/svg" width="19.826" height="14.317" viewBox="0 0 14.826 9.317">
                    <g id="Group_27816" data-name="Group 27816" transform="translate(-785.538 -378.579)">
                        <path id="Path_202457" data-name="Path 202457" d="M792.938,383.516l-6.4-4.937h12.831Z" fill="#545454"/>
                        <path id="Path_202458" data-name="Path 202458" d="M790.717,383.1l-5.179,4.224V379.11Z" fill="#545454"/>
                        <path id="Path_202459" data-name="Path 202459" d="M791.554,383.748l1.382,1.065,1.457-1.12,5.06,4.2H786.468Z" fill="#545454"/>
                        <path id="Path_202460" data-name="Path 202460" d="M795.23,383.051l5.134-3.944v8.206Z" fill="#545454"/>
                    </g>
                    </svg>
            </span>
           </div>
          <div class="auth-input">
            <input type="email" placeholder="E-MAIL ADDRESS" />
            <span>
                <svg xmlns="http://www.w3.org/2000/svg" width="15.685" height="18.27" viewBox="0 0 10.685 13.27">
                    <g id="Group_27805" data-name="Group 27805" transform="translate(-787.115 -434.484)">
                        <path id="Path_202455" data-name="Path 202455" d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z" fill="#545454"/>
                    </g>
                </svg>
            </span>
          </div>
          <div class="auth-input">
            <input type="password" placeholder="PASSWORD" />
            <span>
                <svg xmlns="http://www.w3.org/2000/svg" width="15.685" height="18.27" viewBox="0 0 10.685 13.27">
                    <g id="Group_27805" data-name="Group 27805" transform="translate(-787.115 -434.484)">
                        <path id="Path_202455" data-name="Path 202455" d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z" fill="#545454"/>
                    </g>
                </svg>
            </span>
          </div>
          <div class="auth-input">
            <input type="password" placeholder="CONFIRM PASSWORD" />
            <span>
                <svg xmlns="http://www.w3.org/2000/svg" width="15.685" height="18.27" viewBox="0 0 10.685 13.27">
                    <g id="Group_27805" data-name="Group 27805" transform="translate(-787.115 -434.484)">
                        <path id="Path_202455" data-name="Path 202455" d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z" fill="#545454"/>
                    </g>
                </svg>
            </span>
          </div>
          <div class="auth-submit">
            <button type="submit">LOG IN</button>

               <div class="mt-4">
                  <span>
                    <div class="checkbox">
                        <input id="check1" type="checkbox" name="check" value="check1">
                        <label for="check1">Remember me</label>
                    </div>                        
                  </span>

                  <nuxt-link to="">Forget Password?</nuxt-link>
              </div>
          </div>
        </form>
      </div>
    </div>
    <div class="sidenav-container block screen-67:hidden">
      <div v-if="displaySideNav" class="sidenav-backdrop" @click="displaySideNav=false"></div>
      <transition name="slide-side">
        <div v-if="displaySideNav" @click="displaySideNav=false" class="sidenav overflow-auto">
          <ul class="nav-list">

            <li class="nav-item">
              <nuxt-link to="/" active-class="active-nav-item">
                 <span> homepage</span>
              </nuxt-link
              >
            </li>

           

             <li class="nav-item">
              <nuxt-link to="/shoping" active-class="active-nav-item">
                 <span> shoping</span>
              </nuxt-link
              >
            </li>
           
            <li class="nav-item">
              <nuxt-link to="/blogs" active-class="active-nav-item">
              <span>blogs</span>
               </nuxt-link
              >
            </li>
            <li class="nav-item">
              <nuxt-link to="/events" active-class="active-nav-item">
                 <span>events</span>
              </nuxt-link
              >
            </li>

            <li class="nav-item">
              <nuxt-link to="/contact " active-class="active-nav-item">
                 <span>contact</span>
              </nuxt-link
              >
            </li>
            
          </ul>
        </div>
      </transition>
    </div>
   </div>
</template>

<script>
export default {
  data() {
    return {
      displayAuth: '',
      displaySideNav: false,
    };
  },
  methods: {
    selectAuth(value) {
      this.displayAuth=value;
    },
  }
};
</script>
<style lang="scss" scoped>
#nav {
  @apply flex justify-between items-center py-8 mx-auto;
  max-width: 1918px;
@media only screen and (min-width: 498px) {
      padding-left: 2.5rem;
      padding-right: 2.5rem;
    }
  .side-btn{
    @apply ml-6 flex text-white;
    font-size: 22px;
     @media only screen and (min-width: 1036px) {
      @apply hidden;
    }
  }
  .nav-items {
    @apply flex justify-between items-center text-white;
    .item {
      @apply px-6 flex flex-col items-center justify-center relative;
      a {
        @apply flex-col flex justify-center items-center text-white;
      }
    }
    .active-item {
      .active {
        width: 6rem;
        height: 2px;
        background: linear-gradient(#faab20 0%, #de158c 100%);
        position: absolute;
        bottom: -6px;
      }
    }

    .input-append {
      @apply border border-white text-white outline-none relative hidden;
      border-radius: 5.31px;
      @media only screen and (min-width: 1226px) {
        @apply flex;
      }
      input {
        @apply px-2 py-1 z-10 outline-none;
        background: rgba(185, 185, 185, 0.5);
      }
      ::placeholder {
        color: white;
      }

      .btn-search {
        button {
          @apply absolute;
          border-color: linear-gradient(#f79a2c 0%, #df1e84 100%);
          right: 7px;
          top: 9px;
        }
        .bar {
          @apply absolute;
          height: 32px;
          width: 2px;
          background: linear-gradient(#f79a2c 0%, #df1e84 100%);
          right: 30px;
          top: 0px;
        }
      }
    }

    .shop {
      @apply px-4 hidden;
      @media only screen and (min-width: 548px) {
        @apply flex;
      }
    }
    
    .join-us{
        @apply cursor-pointer flex;
        @media only screen and (max-width: 726px) {
      @apply hidden;
    }
        a{
            @apply w-full;
        }
    }
    .btn {
      @apply px-4 py-1.5  cursor-pointer;
       @media only screen and (min-width: 726px) {
      @apply ml-4;
    }
      border-radius: 12px;
      background: linear-gradient(#f69d29 0%, #df1f84 100%);
    }
  }
  .links {
    @apply hidden;
    @media only screen and (min-width: 1036px) {
      @apply flex;
    }
  }
}
#auth {
    @apply px-8 flex items-center justify-center;
  
  .backdrop {
    @apply w-full h-full fixed left-0 top-0 z-40;
    background-color: rgba(0, 0, 0, 0.7);
  }
.sign-form{
height: 33rem;
}
.login-form{
height: 26rem;
}
  .auth-form {
    @apply w-full relative  z-50 m-auto py-14 px-6 max-w-full;
      @media only screen and (min-width: 419px) {
                  @apply px-12;
            }
            position: fixed;
margin-top: 34rem;

    border-radius: 23px;
    width: 478px;
     background: linear-gradient(to bottom right, #fabd20 0%, #de29a0 100%);

     .active{
         @apply cursor-pointer;
         background: linear-gradient(to right,#dd158b  0%, #f9aa20 100%);
     }
     .btn{
            @apply cursor-pointer;
            background: #d9a59c;
     }
    .auth-btns {
      @apply grid grid-cols-1 justify-items-center gap-6  mb-12;
      @media only screen and (min-width: 419px) {
          @apply grid-cols-2 gap-10;
      }
      a {
        @apply flex items-center justify-center w-full  shadow;
        border-radius: 9.31px;
         min-height: 40px;

      }
    }

    .auth-input {
      @apply mt-6 w-full relative;
      color: #545454;
      input,
      textarea,
      select {
        @apply w-full outline-none pl-14;
        background: rgba(white, 0.5);
        border-radius: 6.09px;
        min-height: 40px;
      }
      span{
          @apply flex justify-center items-center absolute top-0 left-0;
          color: #545454;
        border-radius: 6.09px;
        background: rgba(white, 0.8);
        min-height: 40px;
        min-width: 40px;

      }
      ::placeholder {
        color: #545454;
      }

    }
    .auth-submit{
        @apply flex flex-col items-center justify-center mt-10;
        button{
            @apply w-full shadow;
            height: 39.63px;
            border-radius: 7.61px;
            background: linear-gradient(to right,#f9aa20 0%, #dd158b 100%);
            }

            div{
                @apply flex justify-between items-center text-black text-sm w-full flex-col;
                 @media only screen and (min-width: 419px) {
                  @apply flex-row;
            }
                input{
                    @apply mr-1.5;
                }
            }
            label {
	display: inline-block;
	cursor: pointer;
	position: relative;
	padding-left: 25px;
	margin-right: 15px;
	font-size: 13px;
}
.wrapper {
	width: 500px;
	margin: 50px auto;
}
 input[type=checkbox] {
	display: none;
}
label:before {
	content: "";
	display: inline-block;

	width: 14px;
	height: 14px;
	margin-right: 10px;
	position: absolute;
	left: 0;
	top: 4px;

	background: rgba(36, 36, 36, 0.5);
 }


.checkbox label:before {
    border-radius: 2px;
}

 

input[type=checkbox]:checked + label:before {
	content: "\2713";
	text-shadow: 1px 1px 1px rgba(0, 0, 0, .2);
	font-size: 10px;
	color: #f3f3f3;
	text-align: center;
    line-height: 14px;
}
    }
  }
}
.sidenav-container {
.sidenav-backdrop {
  @apply w-full h-full fixed left-0 top-0 z-50 text-white;
  background-color: rgba(0, 0, 0, 0.7);
}
.sidenav {
  @apply h-full   z-50 fixed top-0 left-0 w-60 text-white;
  background: #1d1d1d;
  @media only screen and (min-width:376px) {
    @apply w-72;
  }
  box-sizing: border-box;
}
.slide-side-enter-active,
.slide-side-leave-active {
  transition: all 0.3s ease-out;
}
.slide-side-enter,
.slide-side-leave-to {
  transform: translateX(-100%);
}
.nav-list {
  list-style: none;
  padding-top: 20px;
  margin: 0;
}
.nav-item {
  @apply flex text-base;
}
.nav-item a {
  text-decoration: none;
  @apply text-lg w-full flex items-center px-6 py-3 text-white;
    
}
.nav-item a:hover,
.nav-item a:active {
    background: -webkit-linear-gradient(#f9aa20 0%, #dd158b 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
 }
.active-nav-item {
    background: -webkit-linear-gradient(#f9aa20 0%, #dd158b 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;}
}

</style>