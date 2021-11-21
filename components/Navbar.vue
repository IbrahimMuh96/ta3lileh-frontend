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
          <a @click="selectAuth('SIGN UP')">join us</a>
        </div>
        <div>
          <a class="btn" @click="selectAuth('LOG IN')">log in</a>
        </div>
        <div class="side-btn">
          <a @click="displaySideNav = !displaySideNav" class="cursor-pointer">
            <i class="fas fa-bars"></i>
          </a>
        </div>
      </div>
    </nav>
    <div id="auth" v-if="displayAuth">
      <div class="backdrop" @click="displayAuth = ''"></div>
      <div
        class="auth-form h-full"
        :class="{
          'login-form': displayAuth == 'LOG IN',
          'sign-form': displayAuth == 'SIGN UP',
        }"
      >
        <div class="auth-btns">
          <a
            :class="{
              active: displayAuth == 'SIGN UP',
              btn: displayAuth != 'SIGN UP',
            }"
            @click="selectAuth('SIGN UP')"
            >SIGN UP</a
          >
          <a
            :class="{
              active: displayAuth == 'LOG IN',
              btn: displayAuth != 'LOG IN',
            }"
            @click="selectAuth('LOG IN')"
            >LOG IN</a
          >
        </div>
        <form action="" v-if="displayAuth === 'LOG IN'">
          <div class="auth-input">
            <input type="email" placeholder="E-MAIL ADDRESS" />
            <span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="19.826"
                height="14.317"
                viewBox="0 0 14.826 9.317"
              >
                <g
                  id="Group_27816"
                  data-name="Group 27816"
                  transform="translate(-785.538 -378.579)"
                >
                  <path
                    id="Path_202457"
                    data-name="Path 202457"
                    d="M792.938,383.516l-6.4-4.937h12.831Z"
                    fill="#545454"
                  />
                  <path
                    id="Path_202458"
                    data-name="Path 202458"
                    d="M790.717,383.1l-5.179,4.224V379.11Z"
                    fill="#545454"
                  />
                  <path
                    id="Path_202459"
                    data-name="Path 202459"
                    d="M791.554,383.748l1.382,1.065,1.457-1.12,5.06,4.2H786.468Z"
                    fill="#545454"
                  />
                  <path
                    id="Path_202460"
                    data-name="Path 202460"
                    d="M795.23,383.051l5.134-3.944v8.206Z"
                    fill="#545454"
                  />
                </g>
              </svg>
            </span>
          </div>
          <div class="auth-input">
            <input type="password" placeholder="PASSWORD" />
            <span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="15.685"
                height="18.27"
                viewBox="0 0 10.685 13.27"
              >
                <g
                  id="Group_27805"
                  data-name="Group 27805"
                  transform="translate(-787.115 -434.484)"
                >
                  <path
                    id="Path_202455"
                    data-name="Path 202455"
                    d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z"
                    fill="#545454"
                  />
                </g>
              </svg>
            </span>
          </div>
          <div class="auth-submit">
            <button type="submit">LOG IN</button>

            <div class="mt-4">
              <span>
                <div class="checkbox">
                  <input
                    id="check1"
                    type="checkbox"
                    name="check"
                    value="check1"
                  />
                  <label for="check1">Remember me</label>
                </div>
              </span>

              <nuxt-link to="">Forget Password?</nuxt-link>
            </div>
          </div>
        </form>
        <form action="" v-if="displayAuth === 'SIGN UP'">
          <div class="auth-input">
            <input type="text" placeholder="USER NAME" />
            <span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="19.826"
                height="14.317"
                viewBox="0 0 14.826 9.317"
              >
                <g
                  id="Group_27816"
                  data-name="Group 27816"
                  transform="translate(-785.538 -378.579)"
                >
                  <path
                    id="Path_202457"
                    data-name="Path 202457"
                    d="M792.938,383.516l-6.4-4.937h12.831Z"
                    fill="#545454"
                  />
                  <path
                    id="Path_202458"
                    data-name="Path 202458"
                    d="M790.717,383.1l-5.179,4.224V379.11Z"
                    fill="#545454"
                  />
                  <path
                    id="Path_202459"
                    data-name="Path 202459"
                    d="M791.554,383.748l1.382,1.065,1.457-1.12,5.06,4.2H786.468Z"
                    fill="#545454"
                  />
                  <path
                    id="Path_202460"
                    data-name="Path 202460"
                    d="M795.23,383.051l5.134-3.944v8.206Z"
                    fill="#545454"
                  />
                </g>
              </svg>
            </span>
          </div>
          <div class="auth-input">
            <input type="email" placeholder="E-MAIL ADDRESS" />
            <span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="15.685"
                height="18.27"
                viewBox="0 0 10.685 13.27"
              >
                <g
                  id="Group_27805"
                  data-name="Group 27805"
                  transform="translate(-787.115 -434.484)"
                >
                  <path
                    id="Path_202455"
                    data-name="Path 202455"
                    d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z"
                    fill="#545454"
                  />
                </g>
              </svg>
            </span>
          </div>
          <div class="auth-input">
            <input type="password" placeholder="PASSWORD" />
            <span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="15.685"
                height="18.27"
                viewBox="0 0 10.685 13.27"
              >
                <g
                  id="Group_27805"
                  data-name="Group 27805"
                  transform="translate(-787.115 -434.484)"
                >
                  <path
                    id="Path_202455"
                    data-name="Path 202455"
                    d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z"
                    fill="#545454"
                  />
                </g>
              </svg>
            </span>
          </div>
          <div class="auth-input">
            <input type="password" placeholder="CONFIRM PASSWORD" />
            <span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="15.685"
                height="18.27"
                viewBox="0 0 10.685 13.27"
              >
                <g
                  id="Group_27805"
                  data-name="Group 27805"
                  transform="translate(-787.115 -434.484)"
                >
                  <path
                    id="Path_202455"
                    data-name="Path 202455"
                    d="M796.639,438.871h-.809v-1.01a3.377,3.377,0,0,0-6.754,0v1.01h-.811a1.155,1.155,0,0,0-1.15,1.149v6.574a1.157,1.157,0,0,0,1.15,1.16h8.374a1.16,1.16,0,0,0,1.161-1.16V440.02A1.158,1.158,0,0,0,796.639,438.871Zm-6.037-1.01a1.851,1.851,0,0,1,3.7,0v1.01h-3.7Zm2.476,6.85v1.68a.126.126,0,0,1-.132.122h-.8a.125.125,0,0,1-.123-.122v-1.68a1.476,1.476,0,1,1,1.059,0Z"
                    fill="#545454"
                  />
                </g>
              </svg>
            </span>
          </div>
          <div class="auth-submit">
            <button type="submit">LOG IN</button>

            <div class="mt-4">
              <span>
                <div class="checkbox">
                  <input
                    id="check1"
                    type="checkbox"
                    name="check"
                    value="check1"
                  />
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
      <div
        v-if="displaySideNav"
        class="sidenav-backdrop"
        @click="displaySideNav = false"
      ></div>
      <transition name="slide-side">
        <div
          v-if="displaySideNav"
          @click="displaySideNav = false"
          class="sidenav overflow-auto"
        >
          <ul class="nav-list">
            <li class="nav-item">
              <nuxt-link to="/" active-class="active-nav-item">
                <span> homepage</span>
              </nuxt-link>
            </li>

            <li class="nav-item">
              <nuxt-link to="/shoping" active-class="active-nav-item">
                <span> shoping</span>
              </nuxt-link>
            </li>

            <li class="nav-item">
              <nuxt-link to="/blogs" active-class="active-nav-item">
                <span>blogs</span>
              </nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link to="/events" active-class="active-nav-item">
                <span>events</span>
              </nuxt-link>
            </li>

            <li class="nav-item">
              <nuxt-link to="/contact " active-class="active-nav-item">
                <span>contact</span>
              </nuxt-link>
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
    }
  },
  methods: {
    selectAuth(value) {
      this.displayAuth = value
    },
  },
}
</script>
<style lang="scss" scoped>
</style>
