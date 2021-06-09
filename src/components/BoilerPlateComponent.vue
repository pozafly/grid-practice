<template>
  <div class="father">
    <div class="child">1</div>
    <div class="child">2</div>
    <div class="child">3</div>
    <div class="child">4</div>
    <div class="child">5</div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.father {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;

  .child {
    flex-basis: 30%;
    background: coral;
    color: #fff;
    font-size: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .child:nth-child(4) {
    margin-top: 10px;
  }
}
</style>
