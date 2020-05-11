<template>
  <div class="block">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'blockComponent'
}
</script>
<style scoped>
  .block {
    width: 98px;
    height: 158px;
    background:#EDF3FF;
    color: #4A4A4A;
    border-radius: 8px;
    margin-left: 10px;
    padding-top: 85px;
    padding-left: 17px;
    box-sizing: border-box;
  }
</style>
