<template>
  <div class="position">
    <div class="tooltips-container">

      <div class="top-container common">

        <Tooltips placement="top-left" content="Top Left Content" >
          <div class="tooltips-content">
            上左
          </div>
        </Tooltips>
        <Tooltips placement="top" content="Top Content">
          <div class="tooltips-content">
            上中
          </div>
        </Tooltips>
        <Tooltips placement="top-right" content="Top Right Content">
          <div class="tooltips-content">
            上右
          </div>
        </Tooltips>
      </div>

      <div class="center-container common">
        <div class="left">
          <Tooltips placement="left-top" content="Left Top Content">
            <div class="tooltips-content">
              左上
            </div>
          </Tooltips>
          <Tooltips placement="left" content="Left Content">
            <div class="tooltips-content">
              左中
            </div>
          </Tooltips>
          <Tooltips placement="left-bottom" content="Left Bottom Content">
            <div class="tooltips-content">
              左下
            </div>
          </Tooltips>
        </div>

        <div class="right">
          <Tooltips placement="right-top" content="Right Top Content">
            <div class="tooltips-content">
              右上
            </div>
          </Tooltips>
          <Tooltips placement="right" content="Right Content">
            <div class="tooltips-content">
              右中
            </div>
          </Tooltips>
          <Tooltips placement="right-bottom" content="Right Bottom Content">
            <div class="tooltips-content">
              右下
            </div>
          </Tooltips>
        </div>
      </div>

      <div class="bottom-container common">
        <Tooltips placement="bottom-left" content="Bottom Left Content">
          <div class="tooltips-content">
            下左
          </div>
        </Tooltips>
        <Tooltips placement="bottom" content="Bottom Content">
          <div class="tooltips-content">
            下中
          </div>
        </Tooltips>
        <Tooltips placement="bottom-right" content="Bottom Right Content">
          <div slot="content"></div>
          <div class="tooltips-content">
            下右
          </div>
        </Tooltips>
      </div>

    </div>
  </div>
</template>

<script>
  import Tooltips from "v-component-tooltips";

  export default {
    name: 'Position',

    components: {
      Tooltips
    },
    data() {
      return {}
    }
  }
</script>

<style lang="scss" scoped>
  .position {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .tooltips-container {
      width: 800px;
      height: 400px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 10px;
      border: 1px solid grey;
      border-radius: 10px;

      .common {
        width: 100%;
        margin: 10px;
      }

      .top-container {
        flex: 1;
      }

      .center-container {
        flex: 3;

        .left {
          float: left;
          display: flex;
          flex-direction: column;
        }

        .right {
          float: right;
          display: flex;
          flex-direction: column;
        }
      }

      .bottom-container {
        flex: 1;
        clear: both;
      }
    }
  }
</style>
