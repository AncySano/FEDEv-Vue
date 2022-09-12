<template>
  <div class="navbar">
    <img
      src="@/assets/ho_me.png"
      srcset="@/assets/ho_me@2x.png 2x, @/assets/ho_me@3x.png 3x"
    />
    <img
      src="@/assets/ho_lo.png"
      srcset="@/assets/ho_lo@2x.png 2x, @/assets/ho_lo@3x.png 3x"
    />
    <img
      src="@/assets/ho_li.png"
      srcset="@/assets/ho_li@2x.png 2x, @/assets/ho_li@3x.png 3x"
    />
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
.navbar {
  width: 100%;
  height: 60px;
  padding: 1rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>