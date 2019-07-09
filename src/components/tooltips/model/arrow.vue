<template>
  <div class="arrow">
    <Tooltips placement="top" content="abc">
      <div class="tooltips-content">
        有箭头
      </div>
    </Tooltips>
    <Tooltips placement="top" content="abc" :no-arrow="true">
      <div class="tooltips-content">
        没有箭头
      </div>
    </Tooltips>
  </div>
</template>

<script>
  import Tooltips from "v-component-tooltips";

  export default {
    name: 'Arrow',

    components: {
      Tooltips
    },
    data() {
      return {}
    }
  }
</script>

<style lang="scss" scoped>
  .arrow {
    width: 800px;
    height: 100px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid grey;
    border-radius: 10px;
  }
</style>
