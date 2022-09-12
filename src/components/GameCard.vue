<template>
  <ul class="game-card">
    <li v-for="(card, index) in gameCardList" :key="index">{{ card }}</li>
  </ul>
</template>

<script>
export default {
  name: "GameCard",
  data() {
    return {
      gameCardList: ["card1", "card2", "card3", "card4"],
    };
  },
};
</script>

<style scoped>
.game-card {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  width: 100%;
  justify-content: space-between;
  padding: 0rem 1rem;
  gap: 1rem;
}

li {
  width: 100px;
  height: 100px;
  background: #efbc42;
  border-radius: 5px;
  text-align: center;
  vertical-align: middle;
  line-height: 150px;
}
</style>