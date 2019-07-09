<template>
  <div class="disabled">
    <Tooltips placement="top" content="有Disabled的content" disabled>
      <div class="tooltips-content">
        有Disabled
      </div>
    </Tooltips>
    <Tooltips placement="top" content="没有Disabled的content">
      <div class="tooltips-content">
        没有Disabled
      </div>
    </Tooltips>
  </div>
</template>

<script>
  import Tooltips from "v-component-tooltips";

  export default {
    name: 'Disabled',

    components: {
      Tooltips
    },
    data() {
      return {}
    }
  }
</script>

<style lang="scss" scoped>
  .disabled {
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
