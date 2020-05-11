<template>
  <div class="window">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'TestObjectivesComponent'
}
</script>
<style>
  .window {
    width: 547px;
    height: 185px;
    background-color: #FFFFFF;
    box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.0212249);
    border-radius: 5px;
    margin-right: 30px;
    padding: 14px;
  }
</style>
