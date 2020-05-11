<template>
  <div class="container">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'UsabilityTestComponent'
}
</script>
<style>
  .container {
    width: 255px;
    padding: 19px;
    background-color: #FFFFFF;;
  }
</style>
