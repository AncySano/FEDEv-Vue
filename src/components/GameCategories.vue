<template>
  <div class="game-categories">
    <!-- categories  -->
    <ul class="category">
      <li
        v-for="(item, index) in category"
        :key="index"
        @click="activeElement = item.name"
      >
        <img
          v-if="activeElement === item.name"
          :src="require(`@/assets/${item.activeSrc}@3x.png`)"
        />
        <img v-else :src="require(`@/assets/${item.inActiveSrc}@3x.png`)" />
      </li>
    </ul>
    <!-- games under category  -->
    <div class="games">
      <div v-for="(item, index) in category" :key="index">
        <ul v-if="activeElement === item.name">
          <li
            class="each-game"
            v-for="(game, vindex) in item.games"
            :key="vindex"
          >
            {{ game }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GameCategories",
  data() {
    return {
      activeElement: "Used",
      category: [
        {
          name: "Used",
          activeSrc: "ho_us1",
          inActiveSrc: "ho_us2",
          games: ["Used Game 1", "Used Game 2", "Used Game 3"],
        },
        {
          name: "Live",
          activeSrc: "ho_li1",
          inActiveSrc: "ho_li2",
          games: ["Live Game 1", "Live Game 2", "Live Game 3"],
        },
        {
          name: "Sport",
          activeSrc: "ho_sp1",
          inActiveSrc: "ho_sp2",
          games: ["Sport Game 1", "Sport Game 2", "Sport Game 3"],
        },
        {
          name: "Lottery",
          activeSrc: "ho_lo1",
          inActiveSrc: "ho_lo2",
          games: ["Lottery Game 1", "Lottery Game 2", "Lottery Game 3"],
        },
        {
          name: "Poker",
          activeSrc: "ho_po1",
          inActiveSrc: "ho_po2",
          games: ["Poker Game 1", "Poker Game 2", "Poker Game 3"],
        },
        {
          name: "Game",
          activeSrc: "ho_ga1",
          inActiveSrc: "ho_ga2",
          games: ["Game 1", "Game 2", "Game 3"],
        },
      ],
    };
  },
};
</script>

<style scoped>
.game-categories {
  width: 100%;
  display: flex;
  gap: 1rem;
  padding: 1rem;
}
/* .category {
  width: 30%;
} */
.category li {
  margin-bottom: 1rem;
}
.games {
  flex: 1;
}
.each-game {
  width: 100%;
  padding: 8px;
  margin-bottom: 8px;
  height: 150px;
  background: #efbc42;
  border-radius: 5px;
  text-align: center;
  vertical-align: middle;
  line-height: 150px;
}
.each-game:hover {
  opacity: 0.9;
}
</style>