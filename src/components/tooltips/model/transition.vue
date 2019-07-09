<template>
  <div class="delay">

    <div class="show-delay">
      <Tooltips placement="top" content="abc" :duration="0.2" transition-function="ease-in">
        <div class="tooltips-content">
          有渐变动画
        </div>
      </Tooltips>
      <Tooltips placement="top" content="abc">
        <div class="tooltips-content">
          没有渐变动画
        </div>
      </Tooltips>
      <Tooltips placement="top" content="abc" :hide-delay="1" :duration="0.2" transition-function="ease-in">
        <div class="tooltips-content">
          有渐变动画和消失延迟
        </div>
      </Tooltips>
    </div>

  </div>
</template>

<script>
  import Tooltips from '../src/index'

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
  .show-delay {
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
