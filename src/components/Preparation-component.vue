<template>
  <div class="section">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'PreparationComponent'
}
</script>
<style>
  .section {
    width: 1130px;
    height: 495px;
    background-color: #FFFFFF;
    box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.0212249);
    border-radius: 5px;
    padding: 26px;
  }
</style>
