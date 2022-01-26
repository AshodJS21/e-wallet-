<template>
  <div id="app">
    <Home v-if="route === 'home'" :cards="cards" @addcard="route = 'newcard'" />
    <NewCard  v-if="route === 'newcard'"
    @card="addCard"  :cards="cards"  :delayTime="delayTime" />
  </div>
</template>

<script>
import Home from "./views/home.vue";
import NewCard from "./views/newCard.vue";
export default {
  components: { Home, NewCard },
  name: "App",
  data() { return {
      delayTime: 2,
      cards: [],
      route: "newcard",
    };
  },

  methods: {
    addCard(card) {
      this.route = "home";
      this.cards.push(card);
      localStorage.setItem("cards", JSON.stringify(this.cards));
    },
  },

  created() {
    let cards = localStorage.getItem("cards");
    if (cards) {
      this.cards = JSON.parse(cards);
    }
  },
};
</script>


<style lang='scss' >
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 10px;

}
</style>

