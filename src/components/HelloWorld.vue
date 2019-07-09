<template>
  <div class="hello">
    <Position></Position>
    <Arrow></Arrow>
    <Delay></Delay>
    <Transition></Transition>
    <Disabled></Disabled>
    <Offset></Offset>
  </div>
</template>

<script>
  import Tooltips from "v-component-tooltips";
  import Position from "./tooltips/model/position"
  import Arrow from "./tooltips/model/arrow";
  import Delay from "./tooltips/model/delay";
  import Disabled from "./tooltips/model/disabled";
  import Offset from "./tooltips/model/offset";
  import Transition from "./tooltips/model/transition";

  export default {
    name: 'HelloWorld',
    components: {
      Tooltips,
      Offset,
      Disabled,
      Delay,
      Arrow,
      Position,
      Transition
    },
    data() {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
</script>

<style lang="scss" scoped>
.hello {
  display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    padding-left: 150px;
}
</style>
