<template>
  <div>
    <h1>ADD A NEW CARD</h1>
    <h6>NEW CARD</h6>
    <br/>
    <article :class="['active-card', this.user.vendor]">
      <div class="top">
        <div class="chip-wifi">
          <svg
            class="wifi-svg"
            width="44"
            height="44"
            viewBox="0 0 44 44"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g opacity="0.5">
              <path
                d="M29.8487 26.501C30.5268 27.1657 30.5268 28.2441 29.8487 28.9097C29.1698 29.5753 28.0694 29.5753 27.3913 28.9097C24.4169 25.9941 19.5778 25.9941 16.6038 28.9097C15.9249 29.5753 14.824 29.5753 14.146 28.9097C13.8068 28.5772 13.6378 28.1423 13.6378 27.7049C13.6378 27.2692 13.8072 26.8331 14.146 26.501C18.4756 22.2567 25.5191 22.2567 29.8487 26.501Z"
                fill="black"
              />
              <path99
                d="M35.8186 21.073C36.4967 21.7382 36.4967 22.817 35.8186 23.4826C35.1397 24.1482 34.0397 24.1482 33.3612 23.4826C27.0956 17.339 16.9004 17.339 10.6348 23.4826C9.95633 24.1482 8.85545 24.1482 8.17785 23.4826C7.83861 23.15 7.66833 22.7135 7.66833 22.2778C7.66833 21.8412 7.83861 21.406 8.17785 21.073C11.869 17.4538 16.7772 15.4608 21.9978 15.4608C27.2184 15.4608 32.1266 17.4538 35.8186 21.073Z"
                fill="black"
              />
              <path
                d="M41.2865 15.0204C41.965 15.6856 41.965 16.7644 41.2865 17.4296C40.608 18.0948 39.508 18.0948 38.8296 17.4296C34.3332 13.0218 28.3554 10.5945 21.9974 10.5945C15.6394 10.5945 9.66196 13.0218 5.16648 17.4296C4.48712 18.0948 3.38712 18.0948 2.70908 17.4296C2.36984 17.097 2.20044 16.6609 2.20044 16.2248C2.20044 15.7891 2.37028 15.353 2.70908 15.0204C7.86104 9.96902 14.7118 7.18753 21.9974 7.18753C29.2842 7.18753 36.1346 9.96902 41.2865 15.0204Z"
                fill="black"
              />
            </g>
          </svg>

          <svg
            class="chip-svg"
            width="50"
            height="40"
            viewBox="0 0 50 40"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect
              width="50"
              height="40"
              rx="8"
              fill="black"
              fill-opacity="0.1"
            />

            <line y1="12.5" x2="18" y2="12.5" stroke="#D0D0D0" />
            <line x1="33" y1="12.5" x2="50" y2="12.5" stroke="#D0D0D0" />
            <line
              x1="32.5"
              y1="5.46392e-08"
              x2="32.5"
              y2="40"
              stroke="#D0D0D0"
            />

            <line y1="26.5" x2="18" y2="26.5" stroke="#D0D0D0" />
            <line x1="32" y1="26.5" x2="50" y2="26.5" stroke="#D0D0D0" />
            <line
              x1="18.5"
              y1="5.46392e-08"
              x2="18.5"
              y2="40"
              stroke="#D0D0D0"
            />
          </svg>
        </div>

        <svg
          class="bitcoin-svg"
          width="28"
          height="39"
          viewBox="0 0 28 39"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M22.497 17.9058C24.5399 16.8521 25.8181 14.9964 25.5195 11.905C25.1174 7.68022 21.5145 6.26356 16.9662 5.86011L16.9653 0H13.4413L13.4403 5.706C12.5132 5.706 11.568 5.72444 10.6271 5.74356L10.6263 0.000777774L7.10548 0.000444465L7.10482 5.85911C6.34178 5.87489 5.59243 5.88989 4.86075 5.88989V5.87256L0 5.87056L0.000657952 9.67967C0.000657952 9.67967 2.60307 9.63011 2.5602 9.67822C3.98706 9.67922 4.45296 10.5181 4.58695 11.2422L4.58805 17.9181V27.2956C4.52522 27.75 4.26086 28.4761 3.26316 28.4774C3.30855 28.5179 0.699671 28.477 0.699671 28.477L0.000657952 32.7364H4.58586C5.44024 32.7374 6.27971 32.7509 7.10329 32.7576L7.10636 38.684L10.6263 38.685L10.6253 32.8207C11.5937 32.8407 12.5285 32.8493 13.4416 32.8481L13.4406 38.685H16.9645L16.9664 32.7684C22.8899 32.424 27.0368 30.9132 27.5524 25.2812C27.968 20.7469 25.8601 18.7229 22.497 17.9058ZM10.7113 9.93678C12.6988 9.93678 18.9494 9.296 18.9503 13.4994C18.9494 17.5293 12.7008 17.0586 10.7113 17.0586V9.93678ZM10.7098 28.5063L10.7113 20.6539C13.0992 20.6532 20.589 19.9582 20.59 24.5783C20.591 29.009 13.0992 28.5046 10.7098 28.5063Z"
            fill="black"
            fill-opacity="0.7"
          />
        </svg>
      </div>

      <div class="middle">
        <span>{{ fillSpan1 }}</span>
        <span>{{ fillSpan2 }}</span>
        <span>{{ fillSpan3 }}</span>
        <span>{{ fillSpan4 }}</span>
      </div>

      <div class="bottom">
        <div>
          <p>Cardholder name</p>
          <p>{{ user.owner ? user.owner : "firstname lastname" }}</p>
        </div>

        <div>
          <p>Valid thru</p>
          <p>{{ fillValid1 }}/{{ fillValid2 }}</p>
        </div>
      </div>
    </article>
    
    <form @submit.prevent="createCard" id="form">
      <label for="number">card number </label>
      <input type="text" id="number" v-model="user.cardNumber" maxlength="16" />

      <label for="number">card holder name </label>
      <input type="text" id="number" v-model="user.owner" maxlength="20" />

      <div>
        <div class="valid">
          <label for="validThru">valid thru</label>
          <input
            type="text"
            id="validThru"
            v-model="user.validThru"
            maxlength="4"
          />
        </div>

        <div class="cvc">
          <label for="cvc">ccv</label>
          <input type="text" id="cvc" v-model="user.cvc" maxlength="4" />
        </div>
      </div>

      <label for="number">vendor</label>

      <select type="options" v-model="user.vendor">
        <option value="ICA">ICA</option>
        <option value="Swedbank">Swedbank</option>
        <option value="AmeriaBank">AmeriaBank</option>
        <option value="HSBC">HSBC</option>
      </select>
      <h5 v-if="showError">* You need to fill out the following requirement</h5>
      <h5 v-if="showNumberError">* Fill out the following requirement with their right characters</h5>
      <input type="submit" />
    </form>
  </div>
</template>

<script>
export default {
  props: ["cards"],

  data() {
    return {
      vendors: ["ICA", "Swedbank", "AmeriaBank", "HSBC"],
      user: {
        owner: "",
        validThru: "",
        cardNumber: "",
        cvc: null,
        vendor: "",
      },
      showError: false,
      showNumberError: false,
    };
  },

  methods: {
    createCard() {
      if (
        !this.user.cardNumber.length <= 0 &&
        !this.user.owner.length <= 0 &&
        !this.user.cvc.length <= 0 &&
        !this.user.vendor.length <= 0 &&
        !this.user.validThru.length <= 0
      ) 
      {
        if (!isNaN(Number(this.user.cardNumber))) {
          const number = this.user.cardNumber.slice(0, 16);
          const card = { ...this.user, cardNumber: number };
          this.$emit("card", card);
          this.showError = false;
          this.user = {
            owner: "",
            validThru: "",
            cardNumber: "",
            cvc: null,
            vendor: "",
          };
          this.showNumberError= false;
        } else {
          this.showNumberError= true;

        }
      } else {
        this.showError = true;
        if (!isNaN(Number(this.user.cardNumber))) {
        
          this.showNumberError= false;
        } else {
          this.showNumberError= true;
        }

      }
    },
  },

  computed: {
    fillSpan1() {
      let span = "";
      for (let i = 0; i < 4; i++) {
        if (this.user.cardNumber[i]) {
          span += this.user.cardNumber[i];
        } else {
          span += "X";
        }
      }
      return span;
    },

    fillSpan2() {
      let span = "";
      for (let i = 4; i < 8; i++) {
        if (this.user.cardNumber[i]) {
          span += this.user.cardNumber[i];
        } else {
          span += "X";
        }
      }
      return span;
    },

    fillSpan3() {
      let span = "";
      for (let i = 8; i < 12; i++) {
        if (this.user.cardNumber[i]) {
          span += this.user.cardNumber[i];
        } else {
          span += "X";
        }
      }
      return span;
    },

    fillSpan4() {
      let span = "";
      for (let i = 12; i < 16; i++) {
        if (this.user.cardNumber[i]) {
          span += this.user.cardNumber[i];
        } else {
          span += "X";
        }
      }
      return span;
    },

    fillValid1() {
      let output = "";
      for (let i = 0; i < 2; i++) {
        if (this.user.validThru[i]) {
          output += this.user.validThru[i];
        } else {
          output += "M";
        }
      }
      return output;
    },

    fillValid2() {
      let output = "";
      for (let i = 2; i < 4; i++) {
        if (this.user.validThru[i]) {
          output += this.user.validThru[i];
        } else {
          output += "Y";
        }
      }
      return output;
    },
  },
};
</script>

<style lang="scss" scoped>
// fix this card changing issues
.active-card {
  background: lightgray;
  width: 382px;
  height: 241px;
  margin: auto;
  border-radius: 8px;
  padding: 16px;
  box-shadow: 0px 0px 8px 5px #0000001f;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
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
}

form {
  max-width: 350px;
  margin: 2rem auto 0 auto;
  text-align: left;
  text-transform: uppercase;
  label {
    display: block;
  }

  input,
  select {
    padding: 1rem;
    display: block;
    width: 100%;
    border-radius: 8px;
    height: 56px;
    margin: 0.1rem 0 1rem 0;
    font-size: 1.3rem;
    border: 1px black solid;
  }

  [type="submit"] {
    background: black;
    height: 72px;
    color: white;
    margin-top: 3rem;
  }

  div {
    display: flex;
    justify-content: space-between;
    div {
      display: flex;
      flex-direction: column;
      width: 45%;
    }
  }
}

.ICA {
  background-color: #8051e6;
  color: #ece6e6;
}

.Swedbank {
  background: #ffb444;
  color: black;
}

.AmeriaBank {
  background: #df2f4e;
  color: black;
}

.HSBC {
  background: #686868;
  color: #ece6e6;
}

h5 {
  color: red;
}
</style>
