<template>
  <div class="containerRow">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'TestTasksComponent'
}
</script>
<style>
  .containerRow {
    width: 195px;
    height: 493px;
    background-color: #F6F9FF;
    margin-left: 20px;
    border-radius: 8px;
    padding: 8px;
  }
</style>
