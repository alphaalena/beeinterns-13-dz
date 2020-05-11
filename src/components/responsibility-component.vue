<template>
  <div class="unit">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'responsibilityComponent'
}
</script>
<style>
  .unit {
    width: 195px;
    height: 240px;
    background-color: #F6F9FF;
    border-radius: 8px;
    margin-bottom: 24px;
    margin-right: 16px;
    padding: 8px;
  }
</style>
