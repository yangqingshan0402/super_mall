<template>
  <div id="tab-bar">
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: "Tabbar",
};
</script>
<style scoped>
#tab-bar {
  height: 49px;
  position: fixed;
  left: 0px;
  bottom: 0px;
  right: 0px;
  /* background-color: green; */
  display: flex;
  align-items: center;
}
</style>
