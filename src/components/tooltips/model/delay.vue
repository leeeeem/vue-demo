<template>
  <div class="delay">

    <div class="delay-box">
      <Tooltips placement="top" content="abc" :show-delay="2">
        <div class="tooltips-content">
          有出现延迟
        </div>
      </Tooltips>
      <Tooltips placement="top" content="abc">
        <div class="tooltips-content">
          没有出现延迟
        </div>
      </Tooltips>
    </div>
    <div class="delay-box">
      <Tooltips placement="top" content="abc" :hide-delay="2">
        <div class="tooltips-content">
          有消失延迟
        </div>
      </Tooltips>
      <Tooltips placement="top" content="abc">
        <div class="tooltips-content">
          没有消失延迟
        </div>
      </Tooltips>
    </div>
    <div class="delay-box">
      <Tooltips placement="top" content="abc" :show-delay="1" :hide-delay="2">
        <div class="tooltips-content">
          有出现和消失延迟
        </div>
      </Tooltips>
    </div>

  </div>
</template>

<script>
  import Tooltips from "v-component-tooltips";

  export default {
    name: 'Delay',

    components: {
      Tooltips
    },
    data() {
      return {}
    }
  }
</script>

<style lang="scss" scoped>
  .delay {
    width: 800px;
    height: 250px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid grey;
    border-radius: 10px;

    .delay-box {
      flex: 1;
    }
  }
</style>
