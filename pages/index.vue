<template>
  <div class="registrationBody">
    <no-ssr>
      <HeaderHero></HeaderHero>
    </no-ssr>
    <div class="container-contact100">
      <div class="wrap-contact100">
        <form class="contact100-form validate-form">
				<span class="contact100-form-title">
					Personal Details
				</span>

          <label class="label-input100" for="first-name">Tell us your name *</label>
          <div class="wrap-input100 rs1-wrap-input100 validate-input" data-validate="Type first name">
            <input id="first-name" class="input100" type="text" name="first-name" placeholder="First name">
            <span class="focus-input100"></span>
          </div>
          <div class="wrap-input100 rs2-wrap-input100 validate-input" data-validate="Type last name">
            <input id="last-name" class="input100" type="text" name="last-name" placeholder="Last name">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="email">Enter your email *</label>
          <div class="wrap-input100 validate-input" data-validate = "Valid email is required: ex@abc.xyz">
            <input id="email" class="input100" type="text" name="email" placeholder="Eg. example@email.com">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="password">Enter your Password *</label>
          <div class="wrap-input100 validate-input" data-validate = "Valid email is required: ex@abc.xyz">
            <input id="password" class="input100" type="password" name="password" placeholder="******">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="phone">Enter phone number</label>
          <div class="wrap-input100">
            <input id="phone" class="input100" type="text" name="phone" placeholder="Eg. +1 800 000000">
            <span class="focus-input100"></span>
          </div>

          <span class="contact100-form-title">
          <br>
					Additional Information
				</span>
          <p style="margin-left: 10px; margin-right: 10px">
            Fill in the below details. This is required to ensure MNO lists your coin with accurate details.
            If you do not have details for required fields, fill in 'TBC' - note that this may delay your listing.
          </p>

          <label class="label-input100" for="coinTicker">Coin Ticker *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="coinTicker" class="input100" name="coinTicker" placeholder="e.g. BTC">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="coinName">Coin Name *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="coinName" class="input100" name="coinName" placeholder="e.g. Bitcoin">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="collateralAmount">Colleteral Amount *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="collateralAmount" class="input100" name="collateralAmount" placeholder="e.g. 1000">
            <span class="focus-input100"></span>
            <hr>
            <p class="description" style="margin-left: 10px"># The masternode collateral requirement for your coin</p>
          </div>

          <div class="wrap-input100 validate-input wrap-checkbox" data-validate = "Coin Ticker is required">
          <span class="span-checkbox">
            <input type="checkbox" id="watchDog" class="input100 checkbox-input" name="watchDog">
            <p style="margin-left: 10px; margin-top: 11px !important;">Pays out on watchdog expired</p>
          </span>
            <span class="focus-input100"></span>
            <hr>
            <p class="description" style="margin-left: 10px; font-style: oblique;">Check if payments include masternodes with watchdog expired</p>
          </div>

          <div class="wrap-input100 validate-input wrap-checkbox" data-validate = "Coin Ticker is required">
          <span class="span-checkbox">
            <input type="checkbox" id="sentinelRequired" class="input100 checkbox-input" name="sentinelRequired">
            <p style="margin-left: 10px; margin-top: 11px !important; padding: 5px;">Sentinel Required</p>
          </span>
            <span class="focus-input100"></span>
            <hr>
            <p class="description" style="margin-left: 10px; font-style: oblique; padding: 5px;">Check if your masternode requires a sentinel to work properly</p>
          </div>

          <label class="label-input100" for="btcTalkAnn">BitcoinTalk ANN *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="btcTalkAnn" class="input100" name="btcTalkAnn" placeholder="e.g. https://bitcointalk.org/index.pxp?topic=421615.0">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="betweenBlocksAnn">BetweenBlocks ANN</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="betweenBlocksAnn" class="input100" name="betweenBlocksAnn" placeholder="e.g. https://betweenblocks.org/topic/58/ann-btc-bitcoin-established-.....">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="github">Github Url *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="github" class="input100" name="github" placeholder="e.g. https://github.com/dashpay/dash">
            <span class="focus-input100"></span>
          </div>

          <div class="wrap-input100 validate-input wrap-checkbox" data-validate = "Coin Ticker is required">
            <p style="margin-left: 10px; font-style: oblique;"># We are unable to list coins without source code.</p>
            <hr>
            <span class="span-checkbox">
            <input type="checkbox" id="sourceCode" class="input100 checkbox-input" name="sourceCode">
            <p style="margin-left: 10px; margin-top: 15px !important;">Yes, source code is available in the repository.</p>
          </span>
            <span class="focus-input100"></span>
          </div>

          <label for="selectxchange" class="label-input100">Listed Exchange *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <select id="selectxchange" class="js-example-basic-multiple selectxchange" name="states[]" multiple="multiple">
              <option value="southxchange">SouthXchange</option>
              <option value="cryptobridge">CryptoBridge</option>
              <option value="cryptopia">Cryptopia</option>
              <option value="btcalpha">BTC-Alpha</option>
              <option value="coinexchange">Coinexchange</option>
              <option value="graviex">Graviex</option>
              <option value="mercatox">MercatoX</option>
              <option value="outletbit">Outletbit</option>
              <option value="bittrex">Bittrex</option>
              <option value="binance">Binance</option>
              <option value="stocksexchange">Stocks.Exchange</option>
              <option value="other">Other</option>
            </select>
            <span class="focus-input100"></span>
            <hr>
            <p class="description" style="margin-left: 10px; font-style: oblique; padding: 5px;">Please select at least 1 exchange your coin is listed on</p>
          </div>


          <label class="label-input100" for="xchgUrl">Exchange URLs</label>
          <div class="wrap-input100 validate-input" data-validate = "Message is required">
            <textarea id="xchgUrl" class="input100" name="xchgUrl"></textarea>
            <span class="focus-input100"></span>
            <hr>
            <p class="description" style="margin-left: 10px; font-style: oblique; padding: 5px;">
              Paste all links to exchange trading pairs here. These must be from exchanges you select above.
            </p>
          </div>

          <label class="label-input100" for="homepage">Homepage *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="homepage" class="input100" name="homepage" placeholder="e.g. https://www.dash.org">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="telegram">Telegram link</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="telegram" class="input100" name="telegram" placeholder="e.g. https://t.me/cto81">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="discord">Discord Chat</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="discord" class="input100" name="discord" placeholder="e.g. https://discord.gg/cto8081">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="twitter">Twitter URL</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="twitter" class="input100" name="twitter" placeholder="e.g. https://twitter.com/Dashpay">
            <span class="focus-input100"></span>
          </div>

          <label class="label-input100" for="blockExplorer">Block Explorer *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="blockExplorer" class="input100" name="blockExplorer" placeholder="e.g. https://explorer.dash.org/chain/Dash">
            <span class="focus-input100"></span>
            <hr>
            <p class="description" style="margin-left: 10px"># Link to your Block Explorer</p>
          </div>

          <label class="label-input100" for="coinLogo">Coin Logo *</label>
          <div class="wrap-input100 validate-input" data-validate = "Coin Ticker is required">
            <input id="coinLogo" class="input100" name="coinLogo" placeholder="e.g. https://www.dash.org/assets/img/graphics/dash_icon_s.png">
            <span class="focus-input100"></span>
            <hr>
            <p class="description" style="margin-left: 10px"># 128x128 PNG direct link to your coin's logo. Any other dimensions or formats will result in lower quality images on MasterNodeum.</p>
          </div>

          <div class="container-contact100-form-btn">
            <a href="#" class="contact100-form-btn" @click="check_empty">
              Place Order
            </a>
          </div>
        </form>

        <div class="contact100-more flex-col-c-m" style="background-image: url('/images/bg-01.jpg');">
          <div class="Order">
            <div class="flex-w size1 p-b-47">
              <div class="txt1 p-r-25">
                <span class="lnr lnr-map-marker"></span>
              </div>

              <div class="flex-col size2">
              <span class="txt1 p-b-20">
                Your Order
              </span>
                <table class="txt3">
                  <thead>
                  <tr>
                    <th><span class="priceTh" >Product</span></th>
                    <th><span class="priceTh" >Total</span></th>
                  </tr>
                  </thead>
                  <tbody>
                  <tr>
                    <td>Product Name Here </td>
                    <td>$100</td>
                  </tr>
                  </tbody>
                  <tfoot>
                  <tr>
                    <th><span class="priceTh" >Subtotal</span></th>
                    <td>$100</td>
                  </tr>
                  <tr style="height: 15px !important;"><td colspan="2"></td></tr>
                  <tr>
                    <th><span class="priceTh" >Total</span></th>
                    <td>$100</td>
                  </tr>

                  </tfoot>
                </table>
              </div>
            </div>




            <!--<div class="flex-w size1 p-b-47">
              <div class="txt1 p-r-25">
                <span class="lnr lnr-map-marker"></span>
              </div>

              <div class="flex-col size2">
                <span class="txt1 p-b-20">
                  Address
                </span>

                <span class="txt2">
                  Mada Center 8th floor, 379 Hudson St, New York, NY 10018 US
                </span>
              </div>
            </div>-->

            <!--<div class="dis-flex size1 p-b-47">
              <div class="txt1 p-r-25">
                <span class="lnr lnr-phone-handset"></span>
              </div>

              <div class="flex-col size2">
                <span class="txt1 p-b-20">
                  Lets Talk
                </span>

                <span class="txt3">
                  +1 800 1236879
                </span>
              </div>
            </div>-->

            <div class="dis-flex size1 p-b-47">
              <div class="txt1 p-r-25">
                <span class="lnr lnr-envelope"></span>
              </div>

              <div class="flex-col size2">
              <span class="txt1 p-b-20">
                General Support
              </span>

                <span class="txt3">
                contact@masternodeum.com
              </span>
              </div>
            </div>



          </div>
        </div>
      </div>
      <!--<script>
        window.onscroll = function() {myFunction()};

        var header = document.getElementById('Order');
        var sticky = header.offsetTop;

        function myFunction() {
          if (window.pageYOffset > sticky) {
            header.classList.add('sticky');
          } else {
            header.classList.remove('sticky');
          }
        }
      </script>-->
      <script>
        $(document).ready(function() {
          $('.selectxchange').select2();
        });
      </script>
    </div>
    <FooterHero></FooterHero>
  </div>
</template>

<script>
  import axios from 'axios'
  import FooterHero from '~/components/FooterHero'
  import HeaderHero from "~/components/HeaderHero";

  export default {
    components: {
      HeaderHero,
      FooterHero
    },
    methods:{
      getSelectedValues (select) {
        let result = [];
        let options = select && select.options;
        let opt;

        for (let i=0, iLen=options.length; i<iLen; i++) {
          opt = options[i];

          if (opt.selected) {
            result.push(opt.value || opt.text);
          }
        }
        return result;
      },
      submit_form () {
        console.log("submitted");
        let data = {
          "firstName": document.getElementById('first-name').value,
          "lastName": document.getElementById('last-name').value,
          "email": document.getElementById('email').value,
          "phone": document.getElementById('phone').value,
          "password": document.getElementById('password').value,
          "coinTicker": document.getElementById('coinTicker').value,
          "coinName": document.getElementById('coinName').value,
          "collateralAmount": document.getElementById('collateralAmount').value,
          "watchDog": document.getElementById('watchDog').checked,
          "sentinelRequired": document.getElementById('sentinelRequired').checked,
          "btcTalkAnn": document.getElementById('btcTalkAnn').value,
          "betweenBlocksAnn": document.getElementById('betweenBlocksAnn').value,
          "github": document.getElementById('github').value,
          "sourceCode": document.getElementById('sourceCode').checked,
          "selectxchange": this.getSelectedValues(document.getElementById('selectxchange')),
          "xchgUrl": document.getElementById('xchgUrl').value,
          "homepage": document.getElementById('homepage').value,
          "telegram": document.getElementById('telegram').value,
          "discord": document.getElementById('discord').value,
          "twitter": document.getElementById('twitter').value,
          "blockExplorer": document.getElementById('blockExplorer').value,
          "coinLogo": document.getElementById('coinLogo').value
        };
        console.log(data);
        axios.post('http://localhost:3000/registration', data)
          .then(response => {
            console.log(response);
            if(response.data.success === true){
              alert("Succesfull");
            }else{
              alert("An Error Encountered");
            }
          }).catch(err => {
          alert("An Error Encountered");
          console.log(err);
        });
        alert("Form Submitted Successfully...");
      },
      check_empty: function () {
        if (
          document.getElementById('first-name').value === "" ||
          document.getElementById('last-name').value === "" ||
          document.getElementById('email').value === "" ||
          document.getElementById('phone').value === "" ||
          document.getElementById('password').value === "" ||
          document.getElementById('coinTicker').value === "" ||
          document.getElementById('coinName').value === "" ||
          document.getElementById('collateralAmount').value === "" ||
          document.getElementById('btcTalkAnn').value === "" ||
          document.getElementById('github').value === "" ||
          document.getElementById('sourceCode').value === "" ||
          this.getSelectedValues(document.getElementById('selectxchange')).length < 1 ||
          document.getElementById('homepage').value === "" ||
          document.getElementById('blockExplorer').value === "" ||
          document.getElementById('coinLogo').value === ""
        ) {
          console.log(this.getSelectedValues(document.getElementById('selectxchange')).toString());
          alert("Fill All Fields !");
        } else {
          this.submit_form();//returnu kaldır
        }
      }
    },
    head () {
      return {
        title: 'MasterNodeum - Registration',
        script: [
          { src: 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js' },
          { src: '../../static/vendor/jquery/jquery-3.2.1.min.js' },
          { src: '../../static/vendor/animsition/js/animsition.min.js' },
          { src: '../../static/vendor/bootstrap/js/popper.js' },
          { src: '../../static/vendor/bootstrap/js/bootstrap.min.js' },
          { src: '../../static/vendor/daterangepicker/moment.min.js' },
          { src: '../../static/vendor/daterangepicker/daterangepicker.js' },
          { src: '../../static/vendor/countdowntime/countdowntime.js' },
          { src: '../../static/js/main.js' },
          { src: 'https://cdnjs.cloudflare.com/ajax/libs/select2/4.0.6-rc.0/js/select2.min.js' }
        ],
        link: [
          { rel: 'stylesheet', href: 'https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css' },
          { rel: 'stylesheet', href: 'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css' },
          { rel: 'stylesheet', href: '../../static/fonts/Linearicons-Free-v1.0.0/icon-font.min.css' },
          { rel: 'stylesheet', href: 'https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.0/animate.min.css' },
          { rel: 'stylesheet', href: 'https://cdnjs.cloudflare.com/ajax/libs/hamburgers/0.9.3/hamburgers.min.css' },
          { rel: 'stylesheet', href: '../../static/vendor/animsition/css/animsition.min.css' },
          { rel: 'stylesheet', href: '../../static/vendor/select2/select2.min.css' },
          { rel: 'stylesheet', href: '../../static/vendor/daterangepicker/daterangepicker.css' },
          { rel: 'stylesheet', href: 'https://cdnjs.cloudflare.com/ajax/libs/select2/4.0.6-rc.0/css/select2.min.css' },
        ],
        build: {
          extractCSS: true
        }
      }
    }
  }
</script>

<style scoped>
  @import "../static/css/main.css";
  @import "../static/css/util.css";
  .checkbox-input{
    width: 3.33% !important;
    margin-left: 25px;
  }

  .span-checkbox{
    display: flex !important;
  }

  .wrap-checkbox{
    margin-top: 15px;
  }
  .input100{
    font-size: 80% !important; /*Düzeltilebilir*/
  }
  .description{
    padding: 5px;
  }
  #selectxchange{
    width: 450px;
  }
  .Order {
    position: fixed;
    top: 25%;
  }
  .priceTh {
    color: #abdde5 !important;
  }
  .registrationBody {
    background: #333;
    background: -webkit-linear-gradient(left top, #ef8e38, #108dc7);
    background: -moz-linear-gradient(bottom right, #ef8e38, #108dc7);
    background: linear-gradient(to bottom right, #ffffcc 0%, #99ccff 116%);
  }
</style>
