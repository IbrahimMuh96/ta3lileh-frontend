<template>
  <div id="index">
    <Navbar> </Navbar>
    <section class="shopping-container">
      <div class="shopping-page-form mr-8">
      <div class="title">
        <img src="../../assets/img/billing-info.svg" alt="" />
      </div>
        <form action="">
             <div class="index-form">
        <div>
          <div class="head">
            <p>How would you like to pay?</p>
            <span class="bar"></span>
          </div>
          <div class="form radio mb-12">
            <div class="container">
                <ul class="list">
                  <li class="list__item">
                    <input type="radio" class="radio-btn" name="choice" id="a-opt" />
                    <label for="a-opt" class="label">Cash on delivery</label>
                  </li>
                  
                  <li class="list__item">
                    <input type="radio" class="radio-btn" name="choice" id="b-opt" />
                    <label for="b-opt" class="label">Credit card</label>
                  </li>
                  
                  <li class="list__item">
                    <input type="radio" class="radio-btn" name="choice" id="c-opt" />
                    <label for="c-opt" class="label">Gift card</label>
                  </li>
                </ul>
          </div>
          
          </div>

          <div class="head">
            <p>Enter Payment Details</p>
            <span class="bar"></span>
          </div>
          <div class="form">
            <div class="index-input">
              <label for=""> Name (as it appears on card) </label>
              <input type="text" />
            </div>
           
            <div class="index-input">
              <label for=""> Card Namber</label>
              <input type="number" />
            </div>

            <div class="payment-info">
              <div class="index-input"  style="width: 9rem;">
                <label for="">MM/YY</label>
                <input type="number" />
              </div>
              <div class="index-input" style="width: 9rem;">
                <label for=""> CVV</label>
                <input type="number" />
              </div>
            </div>
               <div class="index-check mb-12">
               <div class="mt-4">
                    <div class="checkbox">
                        <input id="check1" type="checkbox" name="check" value="check1">
                        <label for="check1">Auto save to billing</label>
                    </div>                        
              </div>
          </div>
          </div>
          <div class="head">
            <p>Billing Address</p>
            <span class="bar"></span>
          </div>
          <div class="form">
            <div class="index-input">
              <label for=""> User Name </label>
              <input type="text" />
            </div>
              <div class="index-input">
              <label for="City"> City</label>
              <select name="" id="City">
                <option value="">Amman</option>
                <option value="">zarqa</option>
              </select>
            </div>
            <div class="index-input">
              <label for=""> Address Description</label>
              <textarea rows="5"></textarea>
            </div>
             <div class="index-input">
              <label for=""> Phone Number</label>
              <input type="text" style="padding-left: 3rem" />
              <span class="">+962</span>
            </div>
            </div>
        </div>
        <div class="float-img">
          <img src="../../assets/img/billing-float.svg" alt="" />
        </div>
      </div>
      </form>
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
              <h1>CONFirM ORDER</h1>
              <span class="bar"></span>
            </div>
            <div class="flex flex-col">
                <div class="total">
                   <p>Subtotal:</p>
                   <p>300 JD</p>
                </div>
                <div class="pay">
                    <span>Pay:</span>
                    <span>
                      credit card
                      as a gift
                    </span>
                </div>

                <div class="confirm-btn">
                  <a href="">CONFIRM</a>
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
 

 
 
</style>