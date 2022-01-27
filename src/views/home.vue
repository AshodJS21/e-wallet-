<template>
  <div>
    <h1>E-Wallet</h1>
    <h6>Active Card</h6>
    <br>
    <div class="active">
      <Card :card="cards[activeCardIndex]" :key="activeCardIndex" />
    </div>

    <div class="collection" v-bind:style="calcDivHeight">
      <Card
        v-for="(card, i) in cards"
        :key="i"
        v-on:click.native="showCard($event, i)"
        :card="card"
        :style="{
          transform: 'translateX(-50%)' + 'translateY(' + i * 4 + 'rem)',
        }"
      />
    </div>

  <button @click="$emit('addcard')">ADD A NEW CARD</button>
  </div>
</template>

<script>
import Card from "../components/card.vue";
export default {
  props: ["cards"],
  components: { Card },

  data() { return {
      activeCardIndex: 0,
      transformX: "translateX(-50%)",
      transformY: "translateY(0)",
    };
  },

  methods: {
    showCard(ev, i) {
      this.activeCardIndex = i;
      console.log("activeCard: ", this.activeCardIndex);
    },
  },

  computed: {
    theActiveCard() {
      return this.cards[this.activeCardIndex];
    },

    calcDivHeight() {
      return {
        minHeight: `calc(241px + (4rem * ${this.cards.length}))`,
      };
    },
  },
};
</script>

<style lang='scss' scoped>
$order: 1;

h1, h6 {
  text-transform: uppercase;
}

h6 {
  color: gray;
  margin: 1rem;
}

.collection {
  position: relative;
  article {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
  }
}

button {
  border: 3px solid black;
  background: white;
  height: 72px;
  width: 350px;
  border-radius: 8px;
  font-size: 1.3rem;
  text-transform: uppercase;
  color: black;
  margin-bottom: 1rem;
  font-weight: bold;
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
</style>

