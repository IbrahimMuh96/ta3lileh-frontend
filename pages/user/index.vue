<template>
  <div id="index">
    <Navbar> </Navbar>
    <section class="section-container">
      <div class="page-form">
      <div class="title">
        <img src="../../assets/img/personal-info.svg" alt="" />
      </div>
        <form action="">
             <div class="index-form">
        <div class="user-img">
          <img src="../../assets/img/defult-profile.png" alt="" />
        </div>
        <div>
          <div class="head">
            <p>About you</p>
            <span class="bar"></span>
          </div>
          <div class="form">
            <div class="index-input">
              <label for=""> User Name </label>
              <input type="text" />
            </div>
            <div class="index-input">
              <label for=""> E-Mail</label>
              <input type="eamil" />
            </div>
            <div class="index-input">
              <label for=""> Phone Number</label>
              <input type="text" style="padding-left: 3rem" />
              <span class="">+962</span>
            </div>

            <div class="index-input" style="width: 13rem">
              <label for=""> Birthday</label>
              <input type="date" />
            </div>

            <div class="index-input" style="width: 7rem">
              <select name="" id="">
                <option value="1">Male</option>
                <option value="0">Female</option>
              </select>
            </div>

            <div class="index-input">
              <label for=""> Address</label>
              <textarea rows="5"></textarea>
            </div>

            <div class="index-input">
              <label for="City"> City</label>
              <select name="" id="City">
                <option value="">Amman</option>
                <option value="">zarqa</option>
              </select>
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
            <p>Enter Payment Details</p>
            <span class="bar"></span>
          </div>
          <div class="form">
            <div class="index-input">
              <label for=""> Name (as it appears on card) </label>
              <input type="text" />
            </div>
            <div class="index-input">
              <label for=""> E-Mail</label>
              <input type="eamil" />
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
            <p>Change The Password</p>
            <span class="bar"></span>
          </div>
          <div class="form">
            <div class="index-input">
              <label for=""> Current Password</label>
              <input type="password" />
            </div>
            <div class="index-input">
              <label for="">New Password</label>
              <input type="password" />
            </div>
            </div>
        </div>
        <div class="float-img">
          <img src="../../assets/img/personal-float.svg" alt="" />
        </div>
      </div>

      <div class="submit-btn">
           <button type="submit">Save Change</button>
      </div>
        </form>
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
 .index-check{

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

	width: 16px;
	height: 16px;
	margin-right: 10px;
	position: absolute;
	left: 0;
	top: 5px;
  color: white;
	background: rgba(219, 219, 219, 0.5);
 }
label{
  color: white;
  font-size: 16px;
}

.checkbox label:before {
    border-radius: 2px;
}

 

input[type=checkbox]:checked + label:before {
	content: "\2713";
	text-shadow: 1px 1px 1px rgba(0, 0, 0, .2);
	font-size: 16px;
	color: #f3f3f3;
	text-align: center;
    line-height: 14px;
}
    }
</style>