<template>
  <article :class="['active-card', this.card.vendor]">
    <div class="top">
      <div class="chip-wifi">

        <svg class="wifi-svg"
          width="44"  height="44"
          viewBox="0 0 44 44"  fill="none"
          xmlns="http://www.w3.org/2000/svg">

        <g opacity="0.5">
          <path  d="M29.8487 26.501C30.5268 27.1657 30.5268 28.2441 29.8487 28.9097C29.1698 29.5753 28.0694 29.5753 27.3913 28.9097C24.4169 25.9941 19.5778 25.9941 16.6038 28.9097C15.9249 29.5753 14.824 29.5753 14.146 28.9097C13.8068 28.5772 13.6378 28.1423 13.6378 27.7049C13.6378 27.2692 13.8072 26.8331 14.146 26.501C18.4756 22.2567 25.5191 22.2567 29.8487 26.501Z"  :fill="wifiFill"  />
          <path  d="M35.8186 21.073C36.4967 21.7382 36.4967 22.817 35.8186 23.4826C35.1397 24.1482 34.0397 24.1482 33.3612 23.4826C27.0956 17.339 16.9004 17.339 10.6348 23.4826C9.95633 24.1482 8.85545 24.1482 8.17785 23.4826C7.83861 23.15 7.66833 22.7135 7.66833 22.2778C7.66833 21.8412 7.83861 21.406 8.17785 21.073C11.869 17.4538 16.7772 15.4608 21.9978 15.4608C27.2184 15.4608 32.1266 17.4538 35.8186 21.073Z"  :fill="wifiFill"  />
          <path  d="M41.2865 15.0204C41.965 15.6856 41.965 16.7644 41.2865 17.4296C40.608 18.0948 39.508 18.0948 38.8296 17.4296C34.3332 13.0218 28.3554 10.5945 21.9974 10.5945C15.6394 10.5945 9.66196 13.0218 5.16648 17.4296C4.48712 18.0948 3.38712 18.0948 2.70908 17.4296C2.36984 17.097 2.20044 16.6609 2.20044 16.2248C2.20044 15.7891 2.37028 15.353 2.70908 15.0204C7.86104 9.96902 14.7118 7.18753 21.9974 7.18753C29.2842 7.18753 36.1346 9.96902 41.2865 15.0204Z"  :fill="wifiFill"  />
        </g>
        </svg>

        <svg  class="chip-svg"
          width="50"  height="40"
          viewBox="0 0 50 40"  fill="none"
          xmlns="http://www.w3.org/2000/svg"  >

        <rect  width="50"  height="40"
            rx="8" :fill="chipFill"
            fill-opacity="0.3"  />

          <line y1="12.5" x2="18" y2="12.5" :stroke="chipLine" />
          <line x1="33" y1="12.5" x2="50" y2="12.5" :stroke="chipLine" />
          <line  x1="32.5"  y1="5.46392e-08"
            x2="32.5"  y2="40"
            :stroke="chipLine"  />

          <line y1="26.5" x2="18" y2="26.5" :stroke="chipLine" />
          <line x1="32" y1="26.5" x2="50" y2="26.5" :stroke="chipLine" />
          <line  x1="18.5"  y1="5.46392e-08"
            x2="18.5"  y2="40"
            :stroke="chipLine"  />
        </svg>
      </div>


    <svg v-if="card.vendor === 'HSBC'"
        class="bitcoin-svg"  height="30"
        viewBox="0 0 28 39"  fill="none"
        xmlns="http://www.w3.org/2000/svg"  >

      <path  d="M22.497 17.9058C24.5399 16.8521 25.8181 14.9964 25.5195 11.905C25.1174 7.68022 21.5145 6.26356 16.9662 5.86011L16.9653 0H13.4413L13.4403 5.706C12.5132 5.706 11.568 5.72444 10.6271 5.74356L10.6263 0.000777774L7.10548 0.000444465L7.10482 5.85911C6.34178 5.87489 5.59243 5.88989 4.86075 5.88989V5.87256L0 5.87056L0.000657952 9.67967C0.000657952 9.67967 2.60307 9.63011 2.5602 9.67822C3.98706 9.67922 4.45296 10.5181 4.58695 11.2422L4.58805 17.9181V27.2956C4.52522 27.75 4.26086 28.4761 3.26316 28.4774C3.30855 28.5179 0.699671 28.477 0.699671 28.477L0.000657952 32.7364H4.58586C5.44024 32.7374 6.27971 32.7509 7.10329 32.7576L7.10636 38.684L10.6263 38.685L10.6253 32.8207C11.5937 32.8407 12.5285 32.8493 13.4416 32.8481L13.4406 38.685H16.9645L16.9664 32.7684C22.8899 32.424 27.0368 30.9132 27.5524 25.2812C27.968 20.7469 25.8601 18.7229 22.497 17.9058ZM10.7113 9.93678C12.6988 9.93678 18.9494 9.296 18.9503 13.4994C18.9494 17.5293 12.7008 17.0586 10.7113 17.0586V9.93678ZM10.7098 28.5063L10.7113 20.6539C13.0992 20.6532 20.589 19.9582 20.59 24.5783C20.591 29.009 13.0992 28.5046 10.7098 28.5063Z"  fill="black"  fill-opacity="0.7"  />
    </svg>

      <svg  v-if="card.vendor === 'Swedbank'"
        height="30"  viewBox="0 0 64 64"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"  >

        <rect width="64" height="64" rx="32" fill="#F33355" />
        <rect  width="64"  height="64"
          rx="32"  fill="url(#paint0_linear_45_5)"
          fill-opacity="0.16"  />
        
        <path  d="M32 49C41.3888 49 49 41.3888 49 32C49 30.0145 48.6596 28.1084 48.034 26.3371C49.9119 23.4372 51 19.9937 51 16.3C51 15.6315 50.0585 15.5682 49.8231 16.1938C48.9585 18.4917 47.6482 20.5767 45.9956 22.3473C42.9283 17.9084 37.8038 15 32 15C26.1962 15 21.0717 17.9084 18.0044 22.3473C16.3518 20.5767 15.0415 18.4917 14.1769 16.1938C13.9415 15.5682 13 15.6315 13 16.3C13 19.9937 14.0881 23.4372 15.966 26.3371C15.3404 28.1084 15 30.0145 15 32C15 41.3888 22.6112 49 32 49ZM26.5138 28.1501C26.9809 27.9801 27.502 28.1791 27.7369 28.6172L30.3917 33.5671C30.8293 34.3831 30.0187 35.3043 29.1537 34.974L21.2205 31.9444C20.3556 31.6141 20.3653 30.3871 21.2354 30.0705L26.5138 28.1501ZM38.2875 28.15C37.8203 27.98 37.2993 28.179 37.0643 28.6171L34.4095 33.567C33.9718 34.3829 34.7825 35.3041 35.6475 34.9738L43.5807 31.9444C44.4456 31.6141 44.4359 30.3871 43.5658 30.0705L38.2875 28.15Z"
          fill="white"  fill-rule="evenodd"  clip-rule="evenodd"  />
        
        
        <defs>
          <linearGradient  id="paint0_linear_45_5"  
            x1="64"  y1="-5.76943e-06"
            x2="-13.2374"  y2="30.7422"
            gradientUnits="userSpaceOnUse"  >
          <stop />

          <stop offset="1" stop-opacity="0" />
          </linearGradient>
        </defs>
      </svg>


      <svg v-if="card.vendor === 'ICA'"
        height="30"  viewBox="0 0 64 64"
        fill="none"  xmlns="http://www.w3.org/2000/svg"  >

        <rect width="64" height="64" rx="32" fill="#8B58F9" />
        <rect  width="64"  height="64"
          rx="32"  fill="url(#paint0_linear_45_4)"
          fill-opacity="0.15" />

        <path  d="M45.3113 18.6979C43.5678 16.9552 41.4272 15.9972 39.284 16C37.2396 16.0029 35.2983 16.8586 33.6985 18.4787L27.719 24.4935C26.0468 26.1738 25.1993 28.1915 25.2685 30.3343C25.3409 32.3969 26.3003 34.4512 27.9689 36.1195C28.9055 37.0554 30.423 37.0554 31.3589 36.1195C32.2955 35.1825 32.2955 33.664 31.3589 32.7288C30.5513 31.9209 30.0899 31.0117 30.0607 30.1728C30.035 29.3788 30.3909 28.6058 31.1186 27.8742L37.0984 21.8597C37.1023 21.8561 37.1059 21.8526 37.1091 21.8487C37.8069 21.1509 38.5417 20.7965 39.2904 20.7951C40.1515 20.794 41.0852 21.2532 41.9217 22.09C42.8715 23.0381 44.1654 24.9299 42.1634 26.9415L39.2248 29.8897C39.1079 30.0073 39.0715 30.223 39.1392 30.3742C39.6181 31.4513 39.8894 32.5819 39.9268 33.7189C39.9429 34.1888 39.9201 34.6527 39.8605 35.1094C39.775 35.7669 40.0006 35.903 40.4681 35.4338L45.5605 30.3246C48.9038 26.9653 48.8011 22.1835 45.3113 18.6979Z"  fill="white"  />
        <path  d="M36.0252 27.9669C35.0883 27.0328 33.5726 27.0345 32.6374 27.9694C31.7001 28.9099 31.7022 30.4277 32.6399 31.3629C33.4485 32.1683 33.9081 33.0757 33.9366 33.9211C33.9637 34.7108 33.6086 35.4831 32.8802 36.2154L26.9018 42.2274C26.8982 42.232 26.8947 42.2348 26.8911 42.2384C26.1923 42.9372 25.4575 43.292 24.7077 43.2938C23.8459 43.2948 22.9107 42.836 22.0768 42.0024C21.1273 41.0526 19.8341 39.1576 21.8332 37.1474L24.7747 34.1985C24.8916 34.0815 24.9276 33.8651 24.8603 33.715C24.3821 32.6393 24.1104 31.5112 24.0709 30.3771C24.0555 29.9054 24.0791 29.4394 24.1393 28.9812C24.226 28.3249 23.9996 28.1872 23.5321 28.6557L18.4365 33.7628C15.0975 37.1192 15.1995 41.9011 18.6861 45.3927C20.431 47.1351 22.572 48.0913 24.7166 48.0885C26.7524 48.0849 28.6763 47.2342 30.2821 45.6291C30.2889 45.622 30.2957 45.6152 30.3025 45.6084L36.2816 39.595C37.9566 37.9093 38.8027 35.8895 38.7285 33.7589C38.6608 31.6934 37.6996 29.6366 36.0252 27.9669Z"  fill="white"  />

        <defs>
          <linearGradient  id="paint0_linear_45_4"
            x1="63.2461"  y1="1.46059"
            x2="-12.8297" y2="31.4021"
            gradientUnits="userSpaceOnUse"  >

        <stop />

        <stop offset="1" stop-opacity="0" />
        </linearGradient>

        </defs>
      </svg>

      <svg v-if="card.vendor === 'AmeriaBank'"
        height="30"  viewBox="0 0 64 64"
        fill="none"  xmlns="http://www.w3.org/2000/svg"  >

        <rect width="64" height="64" rx="32" fill="#222222" />
        <rect  width="64"  height="64"
          rx="32"  fill="url(#paint0_linear_45_3)"
          fill-opacity="0.15"  />
        
        <path  d="M19.5852 21.1465L17.6684 20.3948C16.6913 20.019 16.2403 18.929 16.6161 17.9519C16.9919 16.9747 18.0818 16.5237 19.059 16.8995L20.0362 17.2754L19.7731 16.4109C19.4724 15.4338 20.0362 14.3814 21.0509 14.0808C22.0281 13.7801 23.0805 14.3438 23.3811 15.3586L24.0576 17.6512C26.463 16.4485 29.169 15.7344 32.0253 15.7344C41.4212 15.7344 49.0507 23.3639 49.0507 32.7598C49.0507 42.1557 41.4212 49.7851 32.0253 49.7851C22.6295 49.7851 15 42.1557 15 32.7598C15 28.2873 16.7664 24.1907 19.5852 21.1465ZM44.0145 33.9249C44.0521 33.549 44.0897 33.1732 44.0897 32.7598C44.0897 29.8658 43.0749 27.235 41.3836 25.1679H22.7422C21.0509 27.235 20.0362 29.9034 20.0362 32.7598C20.0362 33.1356 20.0738 33.549 20.1114 33.9249H44.0145Z"  fill="white"  />
        <path  d="M36.9488 32.1209C35.5166 32.1209 34.3555 30.9598 34.3555 29.5276C34.3555 28.0954 35.5166 26.9343 36.9488 26.9343C38.381 26.9343 39.5421 28.0954 39.5421 29.5276C39.5421 30.9598 38.381 32.1209 36.9488 32.1209Z"  fill="white"  />
        <path  d="M27.1019 32.1209C25.6697 32.1209 24.5087 30.9598 24.5087 29.5276C24.5087 28.0954 25.6697 26.9343 27.1019 26.9343C28.5341 26.9343 29.6952 28.0954 29.6952 29.5276C29.6952 30.9598 28.5341 32.1209 27.1019 32.1209Z"  fill="white"  />
        
        <defs>
          <linearGradient  id="paint0_linear_45_3"
            x1="64"  y1="-5.76943e-06"
            x2="-13.2374"  y2="30.7422"
            gradientUnits="userSpaceOnUse">

            <stop stop-color="white" />
            <stop offset="1" stop-color="white" stop-opacity="0" />
          </linearGradient>
        </defs>
      </svg>
    </div>

    <div class="middle">
      <span>{{ span1 }}</span>
      <span>{{ span2 }}</span>
      <span>{{ span3 }}</span>
      <span>{{ span4 }}</span>
    </div>

    <div class="bottom">
      <div>
        <p>Cardholder name</p>
        <p>{{ card.owner }}</p>
      </div>

      <div>
        <p>Valid thru</p>
        <p>{{ valid1 }}/{{ valid2 }}</p>
      </div>

    </div>

  </article>
</template>

<script>
export default {
  props: ["card"],
  data() { return {
      wifiFill: "white",
      chipFill: "black",
      chipLine: "black",
      bgColor: "",
      span1: null,
      span2: null,
      span3: null,
      span4: null,
      valid1: null,
      valid2: null,
    };
  },

  mounted() {
    this.span1 = this.card.cardNumber.slice(0, 4);
    this.span2 = this.card.cardNumber.slice(4, 8);
    this.span3 = this.card.cardNumber.slice(8, 12);
    this.span4 = this.card.cardNumber.slice(12, 16);
    this.valid1 = this.card.validThru.slice(0, 2);
    this.valid2 = this.card.validThru.slice(2, 4);
    switch (this.card.vendor) {
      case "ICA":
        this.wifiFill = "white";
        this.chipFill = "white";
        break;
      default:
        this.wifiFill = "black";
        this.chipFill = "black";
    }
  },
};
</script>


<style lang='scss'>
.active-card {
  background: #FFB444; 
  width: 382px;
  height: 241px;
  margin: 1rem auto;
  border-radius: 8px;
  padding: 16px;
  box-shadow: 0px 0px 8px 5px #0000001F;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  border: 1px solid black;
}

.top {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;

  .bitcoin-svg {
    height: 30px;
    margin-top: 10px;
  }
  .chip-wifi {
    display: flex;
    flex-direction: column;
    .wifi-svg {
      height: 33px;
    }
  }
}

.middle {
  margin: 0.5rem 0 1rem 0;
  display: flex;
  justify-content: space-between;
  span {
    font-size: 1.9rem;
  }
}

.bottom {
  display: flex;
  justify-content: space-between;
  text-transform: uppercase;
  div:first-of-type {
    p:nth-of-type(1) {
      font-size: 0.7rem;
    }
    text-align: left;
  }
  div:last-of-type {
    P:first-of-type {
      font-size: 0.7rem;
    }
  }
}

.ICA {
  background-color: #8051E6;
  color: #ece6e6;
}

.Swedbank {
  background: #FFB444;
  color: black;
}

.AmeriaBank {
  background: #DF2F4E;
  color: black;
}

.HSBC {
  background: #686868;
  color: #ece6e6;
}
</style>
