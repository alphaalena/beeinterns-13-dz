<template>
  <div class="container-plan">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'testPlanComponent'
}
</script>
<style>
  .container-plan {
    width: 659px;
    height: 240px;
    background: #F6F9FF;
    border-radius: 8px;
    padding: 8px;
  }
</style>
