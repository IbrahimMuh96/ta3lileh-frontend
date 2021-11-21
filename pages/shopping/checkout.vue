<template>
  <div id="index">
    <Navbar> </Navbar>
    <section class="shopping-container">
     <div class="shopping-page-form mr-8">
      <div class="title mb-7">
        <img src="../../assets/img/chechout-info.svg" alt="" />
      </div>
      <div>
          <div class="cart">
            <img src="../../assets/img/cart.png" alt="" />

              <h1>NAME OF EVENT</h1>
              <p>
                  <span>Price:&nbsp</span>
                  <span>90 <small>jd</small></span>
              </p>
          </div>
           <div class="cart">
            <img src="../../assets/img/cart.png" alt="" />

              <h1>NAME OF EVENT</h1>
              <p>
                  <span>Price:&nbsp</span>
                  <span>90 <small>jd</small></span>
              </p>
          </div>
           <div class="cart">
            <img src="../../assets/img/cart.png" alt="" />

              <h1>NAME OF EVENT</h1>
              <p>
                  <span>Price:&nbsp</span>
                  <span>90 <small>jd</small></span>
              </p>
          </div>

      </div>
      <div class="cart-btn">
           <a  >Add carts</a>
      </div>
    <div class="float-img">
        <img src="../../assets/img/billing-float.svg" alt="" />
    </div>
    </div>
    <div class="right-index ">
        <div class="steps">
            <div >
             <img src="../../assets/img/steps.svg" alt="" />
             <span class="first_step">STEP 1</span>
             <span class="second_step">STEP 2</span>
             <span class="third_step">STEP 3</span>
            </div>
        </div>
        <div class="card">
            <div class="head">
              <h1>ORDER SUMMARY</h1>
              <span class="bar"></span>
            </div>
            <div class="flex flex-col">
                <div class="total">
                   <p>Subtotal:</p>
                   <p>0 JD</p>
                </div>
                     <div class="index-input">
                        <label for="">Add coupon code:</label>
                        <input type="text" placeholder="Click to add...">
                    </div>
 
                <div class="confirm-btn">
                  <a href="">SUBMIT</a>
                </div>
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
.cart{
    @apply relative flex flex-col items-center justify-center  text-white border-b pb-5 pl-4 border-white mb-7;
     @media only screen and (min-width: 559px) {
        @apply flex-row justify-start;

       }
    max-width: 37rem;
    img{
        border-radius: 5px;
        width: 84.54px;
        height: 66.14px;

        margin-bottom: 7px;
     @media only screen and (min-width: 559px) {
        margin-bottom: 0px;
       }

    }
    h1{
        margin-bottom: 7px;
     @media only screen and (min-width: 559px) {
        @apply ml-4;
        margin-bottom: 0px;
       }
    }
    p{
        background: linear-gradient(to right,#f9aa20 0%, #dd158b 100%);
        border-radius: 9px;
        @apply relative px-2 py-1 flex items-center right-0 cursor-default;
        @media only screen and (min-width: 559px) {
        @apply absolute;

       }
        
         @media only screen and (min-width: 559px) {
        bottom: 13px;
       }
    }
}
  .index-input{
        @apply mb-5 relative mt-8;
        label{
          @apply mb-4 pl-4;
        }

        input,textarea{
          @apply w-full mt-2 px-4;
          -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
          border-radius: 8px;
          min-height: 37px;
          background: rgba(223, 223, 223, 0.4);
          resize: none;
       
        }
        input::-webkit-outer-spin-button,
        input::-webkit-inner-spin-button {
          -webkit-appearance: none;
          margin: 0;
        }

        /* Firefox */
        input[type=number] {
          -moz-appearance: textfield;
        }
        select{
          @apply w-full border border-white px-4 mt-2;
          -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
          padding-top: 7px;
          border-radius: 7px;
          min-height: 37px;
          background: rgba(223, 223, 223, 0.4);
          option{
            color: black;
          }
        }

        span{
          @apply absolute;
          top: 38px;
          left: 8px;
        }
      }
.empty-cart{
    @apply flex items-center text-white mt-6 text-lg;
    margin-left: 5rem;
    img{
       margin-right: 2rem; 
    }
}
$primary-color: #fff;
$accent-color: linear-gradient(#f9aa20 0%, #dd158b 100%);

.cart-btn{
    position: absolute;
bottom: 35px;
right: 22px;

 @media only screen and (min-width: 1231px) {
        right: 50px;

       }
a{
    @apply text-white px-5 py-1.5 cursor-pointer;
    border-radius: 9.82px;
    background: linear-gradient(to right,#f9aa20 0%, #dd158b 100%);
}
}
  .radio{
    .list {
	flex: 0 0 20rem;
}

.list__item {
	position: relative;
	&:hover > .label {
	 
		&::before {
 			margin-right: 2rem;
		}
	}
}

.radio-btn {
	position: absolute;
	opacity: 0;
	visibility: hidden;
	&:checked + .label {
		color: $accent-color;
		&::before {
			 
			border: 4px solid rgba(36, 36, 36, 0.9);
			background: linear-gradient(#f9aa20 0%, #dd158b 100%);
		}
	}
}

 

.label::before {
	display: inline-block;
	content: "";
	height: 1.125rem;
	width: 1.125rem;
	margin-right: 0.625rem;
	border: 1px solid white;
	border-radius: 50%;
	transition: all 0.25s linear;
}
  }
  .right-index{
    @apply flex flex-col relative;
    .steps{
      @apply relative flex-col flex items-center mb-9;
      span{
          @apply absolute text-white text-xl;
      }
      
      .first_step{
          top: 32px;
          left: 52px;
      }
       .second_step{
        top: 32px;
      }
       .third_step{
        top: 32px;
        right: 52px;
      }
    }
      .bar{
          @apply bg-white block mt-2 w-1/2;
           height: 2px;
        }
    .card{
      @apply text-white px-7 py-6 max-w-full; 
      width: 368.91px;
      border-radius: 9.41px;
      background: rgba(36, 36, 36, 0.9);
      .total{
        @apply flex items-center justify-around mt-7;
        p:nth-child(2){
          @apply px-5 py-2;
          border-radius: 9.82px;
background: linear-gradient(#f9aa20 0%, #dd158b 100%);
        }
      }
      .pay{
        @apply mt-5;
        margin-left: 48px;
      }
      .confirm-btn{
        @apply w-full;
       a{
          @apply rounded-full w-full flex items-center justify-center py-1 mt-10;
        background: linear-gradient(to right,#f9aa20 0%, #dd158b 100%);
      
       }
      }
    }
  }
</style>