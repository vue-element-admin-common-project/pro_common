<!-- 页面中 title bar -->
<template>
<div class="comp__title-bar">
  <div class="left-bar"></div>
  <div class="word">{{ title }}</div>
</div>
</template>

<script>
export default {
  name: "TitleBar",
  props: {
    title: { type: String, default: '' }
  }
}
</script>

<style lang="scss" scoped>
@import "~@pro_common/styles/colors.scss";

.comp__title-bar {
  height: 40px;
  display: flex;
  align-items: center;
  background-color: $level-3-border;
  .left-bar {
    width: 10px;
    height: 100%;
    margin-right: 10px;
    background-color: $blue;
  }
  $wordSize: 16px;
  .word {
    font-size: $wordSize;
    line-height: $wordSize;
    color: $level-1-word;
  }
}
</style>
