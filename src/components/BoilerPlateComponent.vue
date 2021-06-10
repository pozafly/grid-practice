<template>
  <div class="father">
    <div class="child">1</div>
    <div class="child">2</div>
    <div class="child">3</div>
    <div class="child">4</div>
    <div class="child">5</div>
    <div class="child">6</div>
    <div class="child">7</div>
    <div class="child">8</div>
    <div class="child">9</div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.father {
  display: grid;
  grid-template-columns: 250px 250px 250px;
  grid-template-rows: 100px 50px 300px;
  gap: 10px;

  .child {
    background: coral;
    color: #fff;
    font-size: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>
