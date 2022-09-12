<template>
  <ul class="footer">
    <li @click="activeElement = 'home'">
      <img
        v-if="activeElement === 'home'"
        src="@/assets/ho_ho1.png"
        srcset="@/assets/ho_ho1@2x.png 2x, @/assets/ho_ho1@3x.png 3x"
      />
      <img
        v-else
        src="@/assets/ho_ho2.png"
        srcset="@/assets/ho_ho2@2x.png 2x, @/assets/ho_ho2@3x.png 3x"
      />
    </li>
    <li @click="activeElement = 'gift'">
      <img
        v-if="activeElement === 'gift'"
        src="@/assets/ho_ac1.png"
        srcset="@/assets/ho_ac1@2x.png 2x, @/assets/ho_ac1@3x.png 3x"
      />
      <img
        v-else
        src="@/assets/ho_ac2.png"
        srcset="@/assets/ho_ac2@2x.png 2x, @/assets/ho_ac2@3x.png 3x"
      />
    </li>
    <li @click="activeElement = 'deposit'">
      <img
        v-if="activeElement === 'deposit'"
        src="@/assets/ho_wa1.png"
        srcset="@/assets/ho_wa1@2x.png 2x, @/assets/ho_wa1@3x.png 3x"
      />
      <img
        v-else
        src="@/assets/ho_wa2.png"
        srcset="@/assets/ho_wa2@2x.png 2x, @/assets/ho_wa2@3x.png 3x"
      />
    </li>
    <li @click="activeElement = 'chat'">
      <img
        v-if="activeElement === 'chat'"
        src="@/assets/ho_co1.png"
        srcset="@/assets/ho_co1@2x.png 2x, @/assets/ho_co1@3x.png 3x"
      />
      <img
        v-else
        src="@/assets/ho_co2.png"
        srcset="@/assets/ho_co2@2x.png 2x, @/assets/ho_co2@3x.png 3x"
      />
    </li>
    <li @click="activeElement = 'profile'">
      <img
        v-if="activeElement === 'profile'"
        src="@/assets/ho_my1.png"
        srcset="@/assets/ho_my1@2x.png 2x, @/assets/ho_my1@3x.png 3x"
      />
      <img
        v-else
        src="@/assets/ho_my2.png"
        srcset="@/assets/ho_my2@2x.png 2x, @/assets/ho_my2@3x.png 3x"
      />
    </li>
  </ul>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      activeElement: "home",
    };
  },
};
</script>

<style scoped>
.footer {
  width: 100%;
  height: 60px;
  padding: 1rem;
  justify-content: space-between;
  align-items: center;
  display: flex;
}
li {
  cursor: pointer;
}
</style>