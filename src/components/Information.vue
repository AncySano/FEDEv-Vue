<template>
  <div class="information">
    <div class="details">
      <img src="@/assets/ho_mo.png" srcset="@/assets/ho_mo@3x.png 3x" />
      <div>
        <div class="subdetails">
          <p>KEN</p>
          <img src="@/assets/ho_vi.png" srcset="@/assets/ho_vi@3x.png 3x" />
          <p class="highlight">7</p>
        </div>
        <div>
          <p class="highlight"><span>$</span>122121233</p>
        </div>
      </div>
    </div>
    <div class="announcement">
      <p>
        <span
          ><img
            src="@/assets/ho_no.png"
            srcset="@/assets/ho_no@2x.png 2x, @/assets/ho_no@3x.png 3x"
        /></span>
        :Dragon Boat Festival holiday!holiday!holiday!holiday!Dragon Boat
        Festival
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Information",
};
</script>

<style scoped>
.information {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem;
}
.details {
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-right: 1px solid #88847d;
  padding-right: 7%;
}
.subdetails {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 2px;
  margin-bottom: 8px;
}
.announcement {
  width: 50%;
  padding-left: 7%;
  position: relative;
}
.announcement p {
  word-break: break-word;
}
p,
span {
  color: #8b8780 !important;
}
.highlight {
  color: #edb845 !important;
}
</style>