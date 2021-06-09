<template>
  <div>
    <div class="msg">
      {{ msg }}
    </div>
    <div class="wrapper">
      <div v-for="count in counts" :key="count">
        <img class="img" src="../../src/assets/logo.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    msg: {
      type: String,
      default: '',
    },
  },

  data() {
    return {
      counts: {
        1: 1,
        2: 2,
        3: 3,
        4: 4,
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.msg {
  color: #fff;
  font-size: 3rem;
}
.wrapper {
  background: darkgray;
  height: 9rem;
  padding: 3rem;
  display: grid;
  grid-template: 100px 100px 100px 100px;
  .img {
    height: 100%;
    background: darkgreen;
  }
}
</style>
