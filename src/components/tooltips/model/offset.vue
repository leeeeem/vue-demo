<template>
  <div class="offset">
    <Tooltips placement="top" content="Top Offset Content" :offset="20">
      <div class="tooltips-content">
        在Top中的位移
      </div>
    </Tooltips>
    <Tooltips placement="bottom" content="Bottom Offset Content" :offset="20">
      <div class="tooltips-content">
        在Bottom中的位移
      </div>
    </Tooltips>
    <Tooltips placement="right" content="Right Offset Content" :offset="20">
      <div class="tooltips-content">
        在Right中的位移
      </div>
    </Tooltips>
    <Tooltips placement="left" content="Left Offset Content" :offset="20">
      <div class="tooltips-content">
        在Left中的位移
      </div>
    </Tooltips>
  </div>
</template>

<script>
  import Tooltips from "v-component-tooltips";

  export default {
    name: 'Offset',

    components: {
      Tooltips
    },
    data() {
      return {}
    }
  }
</script>

<style lang="scss" scoped>
  .offset {
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
